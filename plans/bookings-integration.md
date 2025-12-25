# Plan: Integration of Confirmed Bookings

## Objective
Update all project documentation to align with the hard bookings extracted from `bookings.md`. The bookings reveal significant changes to the assumed itinerary, particularly the route through Europe (Ferry vs Driving) and the dates for West Africa.

## 1. Identified Discrepancies & Changes

| Leg | Current Doc Assumption | Confirmed Booking Reality | Impact |
| :--- | :--- | :--- | :--- |
| **Start** | Jan 16 (Drive from Calais) | **Jan 15** (Ferry from Portsmouth) | Start date shifts earlier. |
| **Europe Route** | Drive through France ("The Sprint") | **Ferry to Santander** (Arrive Jan 17) | **Major Change**. France transit is now a backup. "The Sprint" is removed. |
| **Spain** | Arrive Tarifa Jan 18. Ferry Jan 19. | Stay **Mesón de Sancho** (Cadiz) **Jan 19-21**. Ferry **Jan 21**. | Spain leg is relaxed. Morocco entry delayed 2 days. |
| **Morocco** | Enter Jan 19. Barbas Jan 27. | Enter **Jan 21**. | Morocco leg shifts +2 days. |
| **Mauritania** | Enter Jan 28. | (Implied ~Jan 30/31) | Transit shifts. |
| **Senegal** | Enter Jan 31. Zebrabar Jan 31. | Check-in **Zebrabar Feb 2**. | Senegal entry shifts +2 days. |
| **Senegal Stops** | Zebrabar -> Gambia | **Zebrabar** (Feb 2-4) -> **Somone** (Feb 4-5). | Added stop in Somone. |
| **Gambia** | Enter Feb 2. Finish Feb 6. | Enter **Feb 5**. Stay **Bakadaji** until Feb 11. | Finish line arrival is **Feb 5**. Trip extends to Feb 11. |

## 2. File Update Strategy

### A. `docs/trip-overview.md`
*   **Critical Path**: Update all dates.
    *   Start: Jan 15.
    *   Morocco Entry: Jan 21.
    *   Mauritania/Barbas: Shift estimates (Barbas ~Jan 29/30).
    *   Senegal Entry: Feb 2.
    *   Gambia Entry: Feb 5.
*   **Daily Rhythm**:
    *   **Europe**: Rename "The Sprint" to "The Cruise". Describe the Ferry to Santander + gentle drive to Cadiz.
    *   **West Africa**: Update dates.

### B. `docs/europe-transit.md`
*   **Title**: Update dates (~Jan 15 - Jan 21).
*   **Route**: 
    *   **Primary**: Portsmouth -> Santander Ferry.
    *   **Secondary (Backup)**: Keep the France drive info but mark as "Fallback".
*   **Itinerary**:
    *   Jan 15: Embark Portsmouth.
    *   Jan 17: Arrive Santander. Drive to South? (Santander to Cadiz is ~1000km, 10h drive. Likely a stop needed or a long day. Booking has Check-in Jan 19. Where are we Jan 17-19? *Assumption: Leisurely drive or unbooked stops*).
    *   Jan 19-21: Mesón de Sancho.
    *   Jan 21: Tangier Express.

### C. `docs/morocco.md`
*   **Dates**: Update to Jan 21 - ~Jan 30.
*   **Ferry**: Confirm "Tangier Express" from Algeciras to Tangier Med.
*   **Rally Point**: Adjust Barbas date estimate (likely Jan 30 if we keep the same pace, or tighter driving).

### D. `docs/senegal.md`
*   **Dates**: Feb 2 - Feb 5.
*   **Stops**: 
    *   Zebrabar (Feb 2-4).
    *   **NEW**: Sénébreizh, Somone (Feb 4-5).
*   **Gambia Crossing**: Move to Feb 5.

### E. `docs/the-gambia.md`
*   **Dates**: Feb 5 - Feb 11.
*   **Hotel**: Confirm Bakadaji Hotel details.
*   **Return**: Note flight/end dates.

## 3. Execution Order
1.  Update `trip-overview.md` to set the new baseline.
2.  Reword `europe-transit.md` to reflect the ferry route.
3.  Update Country files (`morocco.md`, `senegal.md`, `the-gambia.md`) with specific dates and venues.
