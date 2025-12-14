# IPL Data Analysis – Power BI Project

## 📌 Project Overview

This project is an **IPL (Indian Premier League) Data Analysis Dashboard** built using **Power BI**. The goal is to analyze IPL match, ball-by-ball, team, and player data to generate meaningful insights such as season-wise performance, team statistics, player achievements, and match outcomes.

The project uses multiple CSV datasets and advanced **DAX measures** to calculate metrics like:

* Matches played and won
* Highest run scorers and wicket takers
* Team-wise and season-wise statistics
* T20-specific analysis
* No-result and tie matches

---

## 📂 Dataset Details

The project is built using the following datasets:

1. **ipl_matches_data11.csv**

   * Match-level information (season, teams, winner, match type, result, venue, etc.)

2. **ball_by_ball_data.csv**

   * Ball-level data (batter, bowler, runs, wickets, sixes, fours, season_id, etc.)

3. **teams_data.csv**

   * Team master data (team_name)

4. **players-data-updated.csv**

   * Player details including player name and image URL

---

## 🛠 Tools & Technologies

* **Power BI Desktop**
* **DAX (Data Analysis Expressions)**
* **CSV Data Sources**


---

## 📊 Key Measures & Insights

### ✔ Match Analysis

* Matches Played by Team (Season-wise, T20 only)
* Matches Won by Team (Season-wise, T20 only)
* Tie Matches Played (Season-wise)
* No Result Matches (Season-wise)

### ✔ Player Performance

* Highest Run Scorer (Season-wise)
* Highest Wicket Taker (Season-wise)
* Total Sixes / Fours by Player
* Player Images using LOOKUPVALUE

### ✔ Team Performance

* Team Matches Played vs Matches Won
* Team-wise T20 Performance
* Team of Highest Run / Wicket Taker

---

## 📈 Dashboard Features

* Interactive slicers (Season, Team)
* Season-wise comparison visuals
* Team & player performance cards
* Clean data modeling with proper relationships

---

## 🔗 Data Modeling

* **teams_data[team_name]** linked with:

  * `ipl_matches_data11[team1]`
  * `ipl_matches_data11[team2]`
  * `ipl_matches_data11[match_winner]`
* `USERELATIONSHIP` and `TREATAS` used where required

---

## 🚀 How to Use

1. Clone this repository
2. Open the Power BI (.pbix) file
3. Ensure CSV files are in the correct path
4. Refresh data
5. Explore dashboards using slicers and visuals

---

## 📌 Notes

* Analysis focuses mainly on **T20 matches**
* Text normalization (`TRIM`, `UPPER`, `LOWER`) is used for accurate filtering
* Boolean fields (like wickets) are handled using `COUNTROWS` logic

---



Happy Analyzing! 📊🏏
