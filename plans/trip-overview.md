# Trip Overview & Operations Plan

**Objective**: Create a high-level operational summary (`docs/trip-overview.md`) focusing on the "Drive" — distances, daily hours, and the critical path to hit the checkpoints on time.

**Secondary Goal**: Calculate average daily drive times and update the "Country Preamble" in each `docs/<country>.md` file to set realistic expectations.

## Phase 1: Route Calculation
**Source**: `docs/_roadbook.txt` and map data.
*   **Segment 1: Europe (The Sprint)**
    *   Calais -> Tarifa. (Highways, fast but long).
*   **Segment 2: Morocco (The Marathon)**
    *   Tangier -> Hotel Barbas. (Scenic slow -> Highway fast).
*   **Segment 3: The Desert (The Challenge)**
    *   Barbas -> Nouakchott. (Border chaos + convoy speeds).
*   **Segment 4: The Finish (The Slog)**
    *   Nouakchott -> Diama -> Banjul. (Bad roads + Borders).

## Phase 2: Create `docs/trip-overview.md`
**Structure**:
```markdown
# Operational Overview: London to Dakar

## The Critical Path
*   **Jan 16**: Start (UK)
*   **Jan 18**: DEADLINE - Tarifa Arrival.
*   **Jan 27**: DEADLINE - Hotel Barbas (Morocco South).
*   **Feb 06**: DEADLINE - Banjul Finish.

## Daily Rhythm
*   **Europe**: High mileage (~800km/day). 8-10 hours driving.
*   **Morocco**: Moderate mileage (~400km/day). 6-8 hours (slower roads/towns).
*   **Sahara**: High mileage (~600km/day). 7-9 hours (straight roads but wind/sand).
*   **West Africa**: Low mileage (~200km/day). 6-8 hours (Terrible roads + Borders).

## Fuel & Logistics Strategy
*   [Fuel Range requirements per section]
*   [Cash strategy per section]
```

## Phase 3: Update Country Preambles
**Target**: Add `**Drive Load**: ~X hrs/day` and `**Distance**: ~Y km` to the header of:
*   `docs/europe-transit.md`
*   `docs/morocco.md`
*   `docs/mauritania.md`
*   `docs/senegal.md`
*   `docs/the-gambia.md`

## Phase 4: Execution
1.  Calculate distances (using `websearch` for realistic travel times, not just "Google Maps perfect world" times).
2.  Create the Overview.
3.  Update the Headers.
