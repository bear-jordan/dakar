# Tourism & Adventure Planning

**Objective**: Populate the "Fun Things to Do" and "Notable Events" sections of the country guides (`docs/<country>.md`). Focus on mid-20s/30s budget travelers interested in culture and nature.

## Phase 1: Roadbook Mining
**Source**: `docs/_roadbook.txt`
*   Identify specific tourist stops mentioned in passing (e.g., Chefchaouen, Dakhla Kitesurfing, St Louis jazz).
*   *Action*: Add these to the relevant country file immediately as "Roadbook Recommended".

## Phase 2: External Research
**Target Audience**: Mid-20s/30s, Budget, Adventure, Cultural.
**Task**: Find 3 relevant travel articles/blogs AND YouTube videos for each country (France, Spain, Morocco, Mauritania, Senegal, The Gambia).
*   *Keywords*: "Road trip stops", "Hidden gems", "Budget adventure", "Off the beaten path".

## Phase 3: Selection & Synthesis
Select **3-5 top recommendations** per country that fit the driving route.
*   **Categorize**: Tag each activity as **[Cultural]**, **[Nature]**, or **[Adventure]**.
*   **Route Check**: Ensure the diversion is reasonable (< 2 hours from main route) or directly on the path.

### Country-Specific Focus Areas
*   **France/Spain**: Quick stops to break up the long drive (e.g., best roadside food, scenic overlooks).
*   **Morocco**: The bulk of the tourism. Focus on the route from Tangier -> Chefchaouen -> Atlas -> Coast.
*   **Mauritania**: Desert experiences that are safe/accessible.
*   **Senegal**: St Louis culture, Pink Lake (if accessible), wildlife.
*   **The Gambia**: River trips, markets, eco-lodges.

## Phase 4: Integration
**Output**: Update `docs/<country>.md`.

**Format Update**:
```markdown
## Fun Things to Do
*   **Activity Name** [Tag]
    *   *Description*: Brief summary.
    *   *Logistics*: "20 min detour from N1".
    *   *Media*: [Video: Title](url) or [Article: Title](url) (Include inline if specific to this activity)

## Recommended Route Adjustments
*   If a specific stop requires a slight route change (e.g., inland via Chefchaouen instead of coastal highway), note it here.

## References
*   [General Country Guide](url)
*   [Vlog Series regarding this region](url)
```

## Execution Steps
1.  Read `docs/_roadbook.txt` for hidden gems.
2.  Perform web searches for "Morocco road trip stops", "Mauritania points of interest", etc.
3.  Update each markdown file with the findings.
