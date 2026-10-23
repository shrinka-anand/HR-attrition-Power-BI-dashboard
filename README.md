# HR-attrition-Power-BI-dashboard
Power BI dashboard analyzing employee attrition (data cleaning, DAX, rate-based visuals)
# HR Attrition Dashboard (Power BI)

![Dashboard](images/dashboard.png)

## Business question
Which employees are most likely to leave, and what do they have in common?

## Data
[Name and source of the dataset, e.g. a public HR analytics dataset]. 1,480 rows raw, 1,470 employees after cleaning.

## What I did
- Removed 7 exact duplicate rows
- Resolved 3 employee IDs with conflicting data
- Fixed a category typo (TravelRarely / Travel_Rarely)
- Created band columns (tenure, distance) and sort columns
- Built DAX measures: Attrition Rate, Attrition Count, Avg Tenure and others
- Used attrition *rates* instead of raw counts, because counts hid the real pattern

## Key findings (16.1% overall attrition)
- Overtime: 30.5% vs 10.4% without overtime
- Age 18-25: 35.8%, the highest of any age group
- Monthly pay up to 5k: 21.8% vs 3.8% for 15k+
- First-year employees: 34.9% vs 8.1% after 10+ years
- Sales Representatives: 39.8%

## Limits
These are associations in one snapshot, not proof of cause. Overtime, age, pay and seniority overlap.

## Files
- `HR_Attrition_Dashboard.pbix`: the Power BI report
- `data/`: cleaned dataset
- `docs/`: cleaning steps and DAX measures

## Tools
Power BI, DAX, Power Query
