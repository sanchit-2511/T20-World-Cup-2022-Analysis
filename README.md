# 🏏 T20 World Cup 2022: Data-Driven Performance Analysis

---

## 🧠 Project Overview

- This project is an end-to-end data analysis solution for the T20 World Cup 2022. It involves data cleaning, transformation, and modeling of match results, player statistics, and ball-by-ball summaries to identify top performers and team trends.

- The goal is to provide a "Manager's View" of player efficiency and team strengths using industry-standard KPIs.

---

## ❓ Analytical Questions

- Who were the most consistent anchors vs. high-impact power hitters in the tournament?

- Which bowlers maintained the best economy rates in the death overs?

- How did different grounds (e.g., Adelaide vs. Perth) impact scoring patterns?

- What was the Win % for teams winning the toss vs. those losing it?

---

## 📁 Dataset Information

- The project uses a structured relational model with the following components:

- Match Dim: Ground, date, teams, and result details.

- Player Dim: Player roles (Batsman/Bowler/All-rounder) and descriptions.

- Batting Fact: Runs, balls faced, boundaries, and strike rates.

- Bowling Fact: Overs, wickets, runs conceded, and economy rates.

---

## 📊 Dashboard Features

- Batting Analytics: Dynamic ranking of players by runs, strike rate, and average.

- Bowling Depth: Analysis of wicket-taking ability vs. run-containment efficiency.

- Ground-Wise Analysis: Insights into how stadium dimensions influenced boundaries and scores.

- Player Selection Tool: Interactive slicers to compare specific players side-by-side.

---

## 🖼️ Dashboard Preview

.

---

## 🔍 Key Insights

- Top Order Dominance: Identified specific players who provided consistent starts vs. those who accelerated in the middle overs.

- Bowling Discipline: Pinpointed bowlers who were effective in "containing" runs during powerplays.

- Critical Success Factors: Teams with a high "Boundary %" showed a strong correlation with winning matches in high-scoring venues.

---

## 🤖 DAX & Metric Engineering

Key measures implemented include:

- Batting Avg: DIVIDE([Total Runs], [Total Innings Dismissed], 0)

- Strike Rate: DIVIDE([Total Runs], [Total Balls Faced], 0) * 100

- Economy Rate: DIVIDE([Runs Conceded], [Overs Bowled], 0)

- Boundary %: Measures the reliance on 4s and 6s for total run tally.

---

## 🛠️ Tools & Technologies Used

- Power BI Desktop: Data Modeling & Dashboarding.

- DAX: For complex calculated measures and columns.

- Power Query: For cleaning "Abandoned" match data and merging player records.

---

## 📂Project Structure
T20-World-Cup-2022-Analysis/
├── Data/
│   ├── dim_match_summary.csv
│   ├── dim_players.csv
│   ├── fact_batting_summary.csv
│   └── fact_bowling_summary.csv
├── Dashboard/
│   └── t20_cricket.pbix             
├── Logic/
│   └── metrics_logic.csv            
│   ├── Batting_Performance.png      
│   ├── Bowling_Insights.png        
│   └── Team_Comparison.png          
└── README.md

---

## 🙌 Author

Sanchit G. Barne

---
