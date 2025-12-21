# Country Logistics & Transit Plan

**Objective**: Create individual practical guides for each country (`docs/<country>.md`) focusing on the *mechanics* of moving the team and vehicle safely through the territory.
**Note**: Exclude "vacation" advice (museums, restaurants) for now. Focus on survival, legality, and progress.

## Phase 1: Structure Definition
For each country (France, Spain, Morocco, Mauritania, Senegal, The Gambia), create/update the specific markdown file with the following logistical sections:

```markdown
# [Country Name] ([Start Date] -- [End Date])
*   **Start Date**: [Date]
*   **End Date**: [Date]
*   **Duration**: [X] Days
*   **Visa**: [Summary Status]

## 1. Pre-Entry Prep
*   **Fuel Strategy**: Fill up before border? (e.g., Cheap fuel in Western Sahara before Mauritania).
*   **Supplies**: Water/Food stocking requirements (e.g., "Dry country" warnings).
*   **Document Staging**: Specific papers to have on the dashboard (Fiche, Insurance, V5).

## 2. Route & Driving Conditions
*   **Mandatory Route**: Key highways or track names mentioned (e.g., "N1").
*   **Hazards**: Animals (camels/goats), speed bumps, unlit roads, sand drifts.
*   **Police/Checkpoints**: Frequency, behavior (friendly vs. corrupt), "Fiche" handing protocol.

## 3. Required Stops
*   **Rally Points**: Specific cities or campsites mentioned as mandatory overnights in the roadbook.
*   **Technical Stops**: Recommended mechanic locations or tire shops.

## 4. Safety & Culture (Practical)
*   **Conduct**: Dress codes, interaction with authorities.
*   **Taboos**: Alcohol rules, photography restrictions (e.g., "No military photos").
*   **Scams**: Specific hustles mentioned in the roadbook (e.g., "The fixer at the border").

## 5. Pre-Exit Checklist
*   **Customs**: What needs to be stamped out?
*   **Currency**: dump local cash?
```

## Phase 2: Extraction Strategy
**Source**: `docs/_roadbook.txt`

1.  **Scan for "Warnings"**: Look for ALL CAPS text or "WARNING" labels in the roadbook regarding driving.
2.  **Map the Stops**: Identify capitalized city names associated with "Day X" or "Night X".
3.  **Border Proximity**: Look for advice specifically given *just before* a new country section starts (usually contains the "Pre-Entry" advice).

## Phase 3: Actionable Tasks (Agent Instructions)
1.  **Create** `docs/morocco.md`, `docs/mauritania.md`, `docs/senegal.md`, `docs/the-gambia.md`.
    *   *Note: France/Spain can be combined or light-touch as they are transit-heavy.*
2.  **Populate** strictly from `docs/_roadbook.txt`.
3.  **Cross-reference** `docs/visas.md` to avoid duplicating strict visa rules, but *do* reference "Preparation" steps like "Have 50 euros in small notes".

## Output
A set of structured markdown files in `docs/` ready for the driving team.
