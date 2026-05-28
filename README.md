# La Liga Historical Data Analysis (1995 - 2025)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data_Manipulation-150458.svg)
![Seaborn](https://img.shields.io/badge/Seaborn-Data_Visualization-3776AB.svg)

## Project Overview

This Exploratory Data Analysis (EDA) investigates 30 years of match outcomes from Spain's top football division, La Liga (1995-1996 season up to Matchday 10 of the 2025-2026 season).

Rather than relying on massive, unwieldy datasets covering all of Europe, this project utilizes a league-specific dataset to streamline analysis and uncover deep, narrative-driven insights about home-field advantage, team consistency, defensive metrics, and the historical dominance of Spain's biggest clubs.

## Key Objectives & Questions Answered

This project is broken down into three distinct analytical phases:

1. **Descriptive Analysis (Foundational):**
   - How much does an empty stadium impact the home-field advantage? _(Analyzed via the 2020-21 pandemic season)._
   - What is the statistical probability of a team holding a halftime lead vs. suffering a comeback?

2. **Comparative Analysis (Intermediate):**
   - How has the goal-difference gap between the "Big Two" (Real Madrid & Barcelona) and the rest of the league evolved?
   - Which La Liga teams are the most statistically consistent, and does consistency correlate with championships?
   - Which teams have the highest ratio of away wins to home wins (Away Day Specialists)?

3. **Predictive & Advanced Modeling (Advanced):**
   - _Historical Recreations:_ Reverse-engineering the historic 2011-12 league table from raw match outcomes.
   - _Metric Creation:_ Engineering a "Clean Sheet" feature to calculate the exact correlation (0.71) between defensive shutouts and final league points.
   - _Performance Decay:_ Visualizing the terminal decline of historic clubs like Deportivo La Coruna to pinpoint the exact season their era ended.

## Highlighted Insights

- **The Halftime Indicator:** Teams leading at halftime in La Liga go on to win the match **75.29%** of the time, while the comeback rate for trailing teams sits at a measly **7.87%**.
- **The Empty Stadium Anomaly:** Without fans in the 2020-21 season, the historical home win rate plummeted by **6%**.
- **The "Centuriones" Math:** By dynamically allocating points (3 for a win, 1 for a draw) to raw historical match data, the logic accurately recreates Real Madrid's record-breaking **100-point** title run in 2011-12.

## Tech Stack

- **Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook

## Dataset Information

- **Source:** UK-based football betting platforms, consolidated into a single master file.
- **Size:** 30 Seasons (1995 - 2025)
- **Key Features:** `Season`, `HomeTeam`, `AwayTeam`, `FTHG` (Full-time home goals), `FTAG` (Full-time away goals), `FTR` (Full-time result), `HTHG` (Half-time home goals), `HTAG` (Half-time away goals), `HTR` (Half-time result).
