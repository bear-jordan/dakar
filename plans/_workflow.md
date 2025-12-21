# Agent Workflow: Autonomous Trip Planning

**Objective**: This document serves as a standard operating procedure (SOP) for an autonomous agent to plan a complex, multi-country road trip from scratch, without a pre-existing "Roadbook."

**Goal**: Create a "Trip Bible" in `docs/` that covers Legal, Logistical, and Cultural requirements for a safe journey.

---

## Phase 1: Architecture & Scope
**Action**: Establish the container for the project.
1.  **Define the Mission**: Create a `README.md` defining:
    *   **Route**: Start point, End point, Transit countries.
    *   **Vehicles**: Type (4x4, Van, Sedan) and ownership (Rental vs. Owned).
    *   **Demographics**: Who is traveling? (e.g., "Mid-30s Budget Adventure").
    *   **Dates**: Start and Finish dates.
2.  **Create Rules**: Create `AGENTS.md` to define output styles (e.g., "No fluff," "Metric system," "Markdown tables").
3.  **Skeleton Files**: Create empty files for each country (e.g., `docs/01-france.md`, `docs/02-spain.md`).

## Phase 2: The "Hard" Gates (Bureaucracy)
**Action**: Determine if the trip is legally possible.
**Tools**: `websearch`, `webfetch` (Gov sources: US State Dept, UK FCDO, Embassies).

1.  **Visa Matrix (`docs/visas.md`)**:
    *   Check entry requirements for the specific passport holders.
    *   Check "Visa on Arrival" vs "E-Visa" vs "Embassy Visit".
2.  **Vehicle Legalities (`docs/car-prep.md`)**:
    *   **Carnet de Passage**: Is it required?
    *   **Insurance**: Green Card zone vs Border Insurance.
    *   **Permits**: International Driving Permits (IDP) requirements (1949 vs 1968 convention).
3.  **Health**:
    *   Mandatory vaccines (Yellow Fever).
    *   Endemic risks (Malaria zones).

## Phase 3: Country Logistics (The "Grind")
**Action**: Populate the country files with survival data.
**Focus**: "How do we move through this country safely?"

For each country, research and log:
1.  **Borders**: Best crossing points (avoiding conflict zones).
2.  **Money**: Cash economy vs Card. Closed currencies? ATM availability.
3.  **Fuel**: Availability, quality (Octane), jerry can laws.
4.  **Connectivity**: Best SIM card provider for rural coverage.
5.  **Police/Corruption**: Checkpoint etiquette, known scams, fines.

## Phase 4: Route & Experience
**Action**: Define the "Line on the Map" and the "Fun".
**Tools**: `websearch` (Blogs, iOverlander, TripAdvisor, Atlas Obscura).

1.  **Route**: Main highways vs Scenic routes. Drive times.
2.  **Stops**:
    *   **Logistical**: Where *must* we sleep (distance limits)?
    *   **Highlights**: Top 3 Cultural/Nature/Adventure stops suitable for the demographic.
3.  **Accommodation Strategy**: Camping culture vs Hotels. (e.g., "Wild camping is illegal in Croatia" vs "Wild camping is mandatory in Mauritania").

## Phase 5: The "Sanity Check" (Forum Mining)
**Action**: Validate static data against recent human experience.
**Source**: Reddit (r/overlanding, r/travel), HUBB (Horizons Unlimited), Facebook Groups.

*   *Prompt*: "Search for 'Morocco border crossing delays 2025' or 'Mauritania fuel shortage'."
*   **Goal**: Find recent changes that official sites missed (e.g., "The bridge is washed out," "Visa fees doubled last week").

## Phase 6: Safety & Emergency
**Action**: Create the safety net.
1.  **Contacts**: Police/Ambulance numbers (they vary by country!).
2.  **Hospitals**: Locate the best *Trauma* center in the capital.
3.  **Diplomacy**: Locate Embassy/Consulate phone numbers.

## Phase 7: Synthesis
**Action**: Generate `docs/_todos.md`.
*   Convert every "Requirement" found in Phases 2-6 into a checkbox task (e.g., "Buy Fire Extinguisher," "Apply for E-Visa").

---

## The Output Template
**File Name**: `docs/[country-name].md`

```markdown
# [Country Name] (~[Start Date] -- [End Date])
*   **Duration**: ~X Days
*   **Visa**: [Summary: VOA / E-Visa / None]
*   **Weather**: [Avg High] / [Avg Low]. [Season Notes]
*   **Currency**: [Name] (1 USD = X). [Cash/Card strategy]

## 1. Pre-Entry Prep
*   **Documents**: [List specific forms/copies needed]
*   **Border Crossing**: [Name of crossing]. [Hours]. [Expected chaos level].
*   **Mandatory Kit**: [Vests, Triangles, Fire Extinguisher, etc.]

### Route Map
| [Country] Road Map |
| :---: |
| ![Map](images/[country]-map.jpg) |

## 2. Route & Driving Conditions
*   **Road Quality**: [Tarmac vs Potholes]
*   **Hazards**: [Animals, Speed bumps, Police traps]
*   **Scams**: [Known local hustles]

## 3. Required Stops / Itinerary
*   **Stop 1**: [City/Location] - [Reason: Sleep/Fuel]
*   **Stop 2**: [City/Location] - [Reason: Activity]

## 4. Safety & Culture (Practical)
*   **Dress Code**: [Modesty requirements]
*   **Taboos**: [Alcohol, Photography, Politics]
*   **Connectivity**: [Best SIM card provider]

## Fun Things to Do
*   **[Activity Name]** [Tag: Nature/Culture]
    *   *Description*: ...
    *   *Logistics*: ...

## Appendix: Emergency & Medical
*   **Emergency**: [Police #] | [Ambulance #]
*   **Key Hospital**: [Name, City]
*   **Embassy**: [Phone #]
```
