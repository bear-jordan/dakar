# Visa & Border Crossing Research Plan

**Objective**: Create a comprehensive `docs/visas.md` file detailing entry requirements, visa costs, and border procedures for the London to Dakar route.

**Target Agent Role**: Research & Documentation Specialist.

## Phase 1: Route Identification
1.  **Analyze `docs/_roadbook.txt`**:
    *   List all countries mentioned in the itinerary order (Start: UK -> Finish: The Gambia).
    *   *Expected List*: UK, France, Spain, Morocco, Western Sahara (disputed), Mauritania, Senegal, The Gambia.

## Phase 2: Roadbook Extraction
**Source**: `docs/_roadbook.txt`
*For each identified country, extract:*
1.  **Visa Status**: Is a visa required? Can it be obtained on arrival (VOA) or must it be done in advance (E-visa/Embassy)?
2.  **Costs**: Extract specific costs mentioned (e.g., "55 euros per person").
3.  **Paperwork/Process**: Look for keywords like "Fiche", "Biometrics", "Photos", "Copies needed".
4.  **Border Specifics**: Note specific border crossings mentioned (e.g., "Diama not Rosso", "Algeciras to Tangier Med").
5.  **Warnings**: scams, bribery attempts, or specific timing advice (e.g., "arrive early").

## Phase 3: Official Verification
**Source**: [US State Department Travel Advisories](https://travel.state.gov/content/travel/en/international-travel/International-Travel-Country-Information-Pages.html) (Search for each country).
*For each country, fetch and record:*
1.  **Official Entry Requirements**: Confirm passport validity rules (e.g., "6 months validity"), number of blank pages.
2.  **Visa Types**: Tourist visa details for US citizens.
3.  **Safety/Advisories**: Summarize "Safety and Security" relevant to driving/border areas (e.g., landmines in Western Sahara/Mauritania border).

## Phase 4: Deliverable Creation
**Output File**: `docs/visas.md`
**Format**:

```markdown
# Visa & Border Crossing Guide

## Summary Table
| Country | Visa Required (US) | Advance/VOA | Approx Cost | Notes |
|---------|-------------------|-------------|-------------|-------|
| ...     | ...               | ...         | ...         | ...   |

## Detailed Country Guides

### [Country Name]
*   **US State Dept Status**: [Level 1-4]
*   **Visa Requirement**: [Details]
*   **Roadbook Advice**:
    *   [Key advice from text]
    *   [Border crossing name]
*   **Critical Alerts**:
    *   [Safety warnings]
```

## Execution Instructions
1.  Run `grep` or `read` on `docs/_roadbook.txt` to find sections matching "Visa", "Border", "Customs".
2.  Use `websearch` or `webfetch` to find the specific US State Dept page for each country (e.g., "Mauritania international travel information site:state.gov").
3.  Synthesize findings into `docs/visas.md`.
