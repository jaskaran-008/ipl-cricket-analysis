# 🏏 IPL Cricket Data Analysis

> Deep-dive analysis of **179,078 ball-by-ball IPL deliveries** across multiple seasons using Python and Pandas — uncovering batting records, bowling dominance, team strategies, and toss impact.

---

## 📊 Dataset

| File | Rows | Columns | Description |
|------|------|---------|-------------|
| `deliveries.csv` | 179,078 | 21 | Ball-by-ball delivery data |
| `matches.csv` | 756 | 18 | Match-level results and metadata |

**Source:** [IPL Dataset — Kaggle](https://www.kaggle.com/datasets/ramjidoolla/ipl-data-set)

---

## 🔍 Analysis Performed

### 1. 🏏 Top Batsmen Analysis
Computed total runs, strike rate, and batting average for every IPL batsman. Filtered and ranked the top 10 all-time run scorers.

| Batsman | Runs | Strike Rate | Batting Avg |
|---------|------|-------------|-------------|
| V Kohli | 5,434 | 129.04 | 35.75 |
| SK Raina | 5,415 | 133.90 | 33.63 |
| RG Sharma | 4,914 | 128.77 | 30.33 |
| DA Warner | 4,741 | 139.52 | 41.59 |
| AB de Villiers | 4,428 | **148.74** | 42.58 |

> **Key Insight:** AB de Villiers has the highest strike rate (148.74) among the top 10 — scoring nearly 1.5 runs per ball. V Kohli leads in total runs but SK Raina is just 19 runs behind.

---

### 2. 🎳 Top Bowlers Analysis
Filtered bowlers with at least 200 balls bowled. Computed wickets taken (excluding run-outs), economy rate, and ranked by wickets.

| Bowler | Wickets | Economy | Balls |
|--------|---------|---------|-------|
| SL Malinga | 170 | 7.08 | 2,974 |
| A Mishra | 156 | 7.28 | 3,172 |
| Harbhajan Singh | 150 | 7.04 | 3,451 |
| R Ashwin | 125 | **6.75** | 3,016 |
| SP Narine | 122 | **6.78** | 2,600 |

> **Key Insight:** SL Malinga dominates with 170 wickets — 14 more than 2nd place. R Ashwin has the best economy among top wicket-takers (6.75 runs/over).

---

### 3. 🏆 Team Win Rate Analysis
Calculated overall win percentage for each franchise based on matches played.

| Team | Win Rate |
|------|----------|
| Delhi Capitals | 62.5% |
| Rising Pune Supergiant | 62.5% |
| Chennai Super Kings | 60.97% |
| Mumbai Indians | 58.29% |
| Royal Challengers Bangalore | 46.67% |

> **Key Insight:** CSK and MI are the most consistent franchises across seasons. RCB with some of cricket's biggest names sits below 47% win rate.

---

### 4. 📈 Batting First vs Chasing Strategy
Analyzed win rates for each team when batting first (winning by runs) vs chasing (winning by wickets).

> **Key Insight:** Gujarat Lions win 40% of matches when chasing but only 3.3% when batting first — extreme specialists. CSK is most balanced: 31.7% batting first, 29.3% chasing.

---

### 5. 🎲 Toss Impact Analysis
Measured the rate at which teams win the toss, choose to bat, AND win the match.

> **Key Insight:** CSK leads at 18.3% — winning toss → batting first → winning match. Gujarat Lions, Kochi Tuskers, and Rising Pune Supergiant: 0% success rate with this approach.

---

## 📈 Visualizations

| Chart | Description |
|-------|-------------|
| Top 10 Batsmen by Runs | Bar chart — V Kohli leads, Raina close behind |
| Top 10 Bowlers by Wickets | Bar chart — Malinga's dominance is clear |
| Top 10 Teams by Win Rate | Bar chart — Delhi Capitals and RPS surprise at top |
| Win Rate When Chasing | Bar chart — Gujarat Lions are chase specialists |
| Toss + Bat First + Win Rate | Bar chart — CSK's strategic consistency |

---

## 🛠️ Tools & Libraries

```
Python 3.x
├── pandas       — data loading, filtering, groupby, aggregation
├── numpy        — vectorized operations
└── matplotlib   — bar chart visualizations (5 charts)
```

---

## ▶️ How to Run

```bash
# 1. Clone the repo
git clone https://github.com/jaskaran-008/ipl-cricket-analysis.git
cd ipl-cricket-analysis

# 2. Install dependencies
pip install pandas numpy matplotlib

# 3. Add datasets (download from Kaggle link above)
#    Place deliveries.csv and matches.csv in the root folder

# 4. Open the notebook
jupyter notebook ipl_analysis.ipynb
```

---

## 🧠 What This Demonstrates

- Loading and exploring large datasets (179K+ rows) with Pandas
- `groupby()` with named aggregations (`agg()`) for multi-metric analysis
- Boolean masking with multiple conditions for precise filtering
- Computing derived metrics (strike rate, economy rate, win %)
- `pd.concat()` for combining multiple Series into analysis DataFrames
- Clean, reproducible Jupyter notebook with markdown documentation
- Matplotlib bar charts with custom colors, gridlines, and formatting

---

## 📁 Project Structure

```
ipl-cricket-analysis/
├── ipl_analysis.ipynb      ← Main analysis notebook
├── deliveries.csv          ← Ball-by-ball data (179K rows)
├── matches.csv             ← Match results (756 rows)
└── README.md
```

---

## 👤 Author

**Jaskaran Singh** — Aspiring Data Analyst | Python · SQL · Pandas · Power BI  
📍 Chandigarh/Mohali Region  
🔗 [LinkedIn](https://linkedin.com/in/yourprofile) · [GitHub](https://github.com/jaskaran-008)

---

*Part of my 12-week Data Science internship preparation roadmap. Week 2 of 12.*