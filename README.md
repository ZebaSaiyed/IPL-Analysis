# 🏏 IPL Data Analysis (2008–2024)

## About This Project
This project presents a complete Exploratory Data Analysis (EDA) 
of Indian Premier League (IPL) matches from 2008 to 2024, 
including player performance analysis and a Machine Learning 
model for match win prediction.

## Dataset
- **Source:** Kaggle
- **matches.csv** — 1095 matches across 17 seasons
- **deliveries.csv** — 260,920 ball by ball records
- > **Note:** deliveries.csv (27.5MB) is not uploaded due to size. 
> Download it from Kaggle: https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020

## Tools Used
Jupyter Notebook | Python | Pandas | NumPy | Matplotlib | Seaborn | Scikit-learn | SQLite
## View Notebook Online
👉 View IPL_EDA.ipynb on nbviewer.
> **Link:** https://nbviewer.org/github/ZebaSaiyed/IPL-Analysis/blob/main/IPL_EDA.ipynb 

## Project Structure
- Team Performance | Toss Analysis | Season Trends
- Top Batsmen | Strike Rate | Top Bowlers | Economy Rate
- Statistical Summary
- Match Win Prediction (ML Model)
- SQL Analysis (7 queries using SQLite)

## How to Run
1. Clone or download this repository
2. Make sure **matches.csv** and **deliveries.csv** are in the same folder as **IPL_EDA.ipynb**
3. Open **IPL_EDA.ipynb** in Jupyter Notebook
4. Run cells using **Shift + Enter** or the **Run** button
5. **Note:** Run all import cells first before running analysis cells

## Key Findings
- **Mumbai Indians** dominate with 144 wins — most successful IPL team
- **Virat Kohli** leads runs (8014) and boundaries (981)
- **Yuzvendra Chahal** leads wickets with 213
- **Sohail Tanvir** has best economy rate at 6.23
- Top 10 strike rates dominated by overseas players — only **Shashank Singh** represents India
- **Sunil Narine** is the only active bowler in top 10 of both wickets and economy
- Spinners dominate bowling — only **Bumrah and Malinga** as pace bowlers in top 10
- Both **Chris Gayle** and **AB de Villiers** in top 10 batsmen — both from RCB

## Results
- Total matches analyzed: **1095**
- Seasons covered: **17 (2008–2024)**
- Teams: **19**
- ML Model Accuracy: **24.77%**
- Average matches per season: **64.41**
- Highest run scorer: **V Kohli (8014 runs)**
- Most wickets: **YS Chahal (213 wickets)**


## SQL Analysis

Performed structured queries using SQLite to extract insights, including multi-table JOINs combining match and delivery-level data:

- Most wins by team (all time)
- Most wins batting first
- Top venues by matches played
- Highest average target runs by season
- Top 10 run scorers (using ball-by-ball data)
- Top 10 wicket takers (using ball-by-ball data)
- Team totals at Eden Gardens *(JOIN — matches + deliveries)*
- Batter performance by venue, highlighting home-ground trends *(JOIN — matches + deliveries)*
  

## Key SQL Insights

- **Mumbai Indians** dominate overall with most wins, but **Chennai Super Kings** are the best "bat first and win" team with 35 wins
- **Eden Gardens** is the most used IPL venue with 77 matches
- IPL scoring has increased significantly — 2024 had the highest average target of 190+ runs
- **Virat Kohli** leads all-time run scoring with 8,014 runs
- **YS Chahal** is the highest wicket taker with 213 wickets
- **Kolkata Knight Riders** dominate their home ground, posting the highest single-innings totals at Eden Gardens (232, 218, 203 runs) — home advantage clearly reflected in the data
- Batter-venue analysis reveals strong "home ground" patterns — **Virat Kohli** (1,874 runs at M. Chinnaswamy Stadium), **Rohit Sharma** (1,733 runs at Wankhede), and **MS Dhoni/Suresh Raina** (1,145/1,302 runs at MA Chidambaram Stadium) all rack up their highest totals at their own team's home venue
- Data quality issue found: Wankhede Stadium appears under two different names in the dataset



## Minor Project — Power BI Dashboards
Three interactive dashboards built using Microsoft Power BI:

| Dashboard | Dataset Source |
|-----------|---------------|
| IPL_Dashboard.pbix | Kaggle — IPL Complete Dataset (Same matches and deliveries dataset i used for EDA) |
| Ecommerce_Dashboard.pbix | Kaggle — Ecommerce Sales Data |
| COVID_Dashboard.pbix | Kaggle — covid-19-india by sudalairajkumar |

**Links for the Ecommerce & Covid datasets**
> Ecommerce: https://www.kaggle.com/datasets/uzmaakhtar/ecommerce-sales-data

> Covid: https://www.kaggle.com/datasets/sudalairajkumar/covid19-in-india 

> **Note:** To view dashboards, download .pbix files and open 
> in Microsoft Power BI Desktop (free). PDF previews also available.


## Author
~ *Zeba Saiyed*

---
*"At the end, cricket is an unpredictable game. It starts from 
the silence of a toss and ends with a nail biting six or a wicket. 
Enjoying it without having a heart attack is itself an ART!"* 🏏❤️
