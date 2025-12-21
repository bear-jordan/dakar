# WhatsApp Intelligence Mining Plan

**Objective**: Parse the unstructured chat history in `docs/whatsapp/_chat.txt` to uncover real-time updates, warnings, and tips that may contradict or supplement the static Roadbook.

**Output**: Create temporary files `docs/<country>-whatsapp.md` and `docs/general-whatsapp.md` containing categorized findings.

## Phase 1: Ingestion & Chunking
**Source**: `docs/whatsapp/_chat.txt`
*   **Method**: Read the file content. If the file is extremely large (>2000 lines), process it in chunks to avoid context limits.
*   **Filtering**: 
    *   **Primary Filter**: **STRICTLY** focus on messages from `~David Clement` or `~Elaine Clement` (Trip Leaders).
    *   **Secondary**: Only include other users if they are directly answering a question *confirmed* by David/Elaine.
    *   Ignore "joined using group link", "added you", and general pleasantries.

## Phase 2: Keyword Scanning & Extraction
Scan the conversation for these specific domains:

### 1. Border & Visa Intelligence
*   *Keywords*: "Visa", "Border", "Cost", "Bribe", "Dahid", "Moulaye", "Form", "Reject", "Euro", "Change".
*   *Goal*: Identify specific costs (e.g., "Paid 55 euros not 50"), time delays, or procedure changes (e.g., "Biometrics now required").

### 2. Route & Logistics
*   *Keywords*: "Road", "Police", "Stop", "Fine", "Hotel", "Fuel", "Gas", "Speed", "Trap", "Maps".
*   *Goal*: Find recommendations for specific mechanics, warnings about specific police checkpoints (e.g., "The bad cop at Thies"), or road conditions.

### 3. Car Prep & Breakdowns
*   *Keywords*: "Breakdown", "Tyre", "Sump", "Overheat", "Fix", "Mechanic", "Part", "Tool".
*   *Goal*: Real-world failure points (e.g., "Roofs collapsing") and fix solutions.

### 4. Gear & Tips
*   *Keywords*: "Bring", "Wish", "Cold", "Hot", "Food", "Sim", "Data", "Signal", "Money".
*   *Goal*: Practical advice from the field (e.g., "Starling card didn't work in Mauritania").

## Phase 3: Output Generation
Create the following files. **Do not overwrite existing docs yet**. We will review these temporary files first.

*   `docs/general-whatsapp.md`: Car prep, gear, general money tips.
*   `docs/morocco-whatsapp.md`
*   `docs/mauritania-whatsapp.md`
*   `docs/senegal-whatsapp.md`
*   `docs/gambia-whatsapp.md`

**Format for Output Files**:
```markdown
# [Country] WhatsApp Intel

## Visas & Borders
*   [Date] User: "Quote or summary of advice"

## Logistics (Fuel/Hotels)
*   [Date] User: "..."

## Safety/Police
*   [Date] User: "..."
```

## Phase 4: Execution Strategy
1.  Read `docs/whatsapp/_chat.txt`.
2.  Synthesize the notes into the relevant buckets.
3.  If a message contradicts the Roadbook, mark it as **[CONFLICT]**.
