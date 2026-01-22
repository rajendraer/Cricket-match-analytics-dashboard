# 🏏 Cricket Match Analytics Dashboard (Power BI)

This project is a Power BI dashboard that provides insights into cricket matches including total matches, live matches, upcoming matches, and finished matches.

## 📌 Features
- KPI Cards:
  - Total Matches
  - Live Matches
  - Upcoming Matches
  - Finished Matches
  - Last Updated Time
- Match details table with team and score information
- Donut chart showing match distribution by status
- Bar chart showing top teams played
- Interactive slicers:
  - Match Status
  - Team 1
  - Team 2

## 🧠 DAX Measures Used
Example:
```DAX
Live Matches =
CALCULATE(
    COUNT(matches[matchId]),
    matches[status] = "Live"
)
