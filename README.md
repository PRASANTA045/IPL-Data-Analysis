
## 🏏 IPL Data Analysis Project

### 📌 Overview

This project is a comprehensive analysis of the Indian Premier League (IPL) dataset from 2008 to 2024, covering both **ball-by-ball (`deliveries.csv`)** and **match-level (`matches.csv`)** data. The goal is to extract deep insights about teams, players, matches, and performance trends through systematic data cleaning, transformation, and visual exploration.

---

### 📁 Datasets Used

* `deliveries.csv`: Ball-by-ball data of every IPL match
* `matches.csv`: Match-level summary information

---

### 🧹 Step 1: Data Cleaning & Preprocessing

#### ✅ Deliveries Data (`deliveries.csv`)

* **Handled Null Values:**

  * `extras_type`: filled with `'Noextra'`
  * `player_dismissed`: filled with `'Noone'`
  * `dismissal_kind`: filled with `'notout'`
  * `fielder`: filled with corresponding `bowler` if missing
* **Renamed Columns:**

  * `match_id` → `id`
* **Standardized Team Names:**
  Converted full team names like `"Chennai Super Kings"` → `"CSK"` in `batting_team` and `bowling_team`
* **Removed Duplicates** (if any)

#### ✅ Matches Data (`matches.csv`)

* **Handled Null Values:**

  * Filled `city` using `venue` column
  * Filled missing `player_of_match` by selecting top run-scorer from that match
  * Calculated missing `result_margin` from innings scores
  * Replaced missing `winner` with `'unknown'` and `method` with `'No D/L'`
* **Removed Completely Empty Records**
* **Standardized Team Names** across `team1`, `team2`, `toss_winner`, `winner`, etc.

---

### 📊 Step 2: Exploratory Data Analysis (EDA)

Here are some key analysis and visualizations performed:

#### 🏆 Team Performance

* Win percentage by team
* Most successful teams over the years
* First innings vs second innings performance

#### 🎯 Player Performance

* Top run scorers
* Highest wicket takers
* Most fours and sixes
* Best strike rates and economy

#### 🧠 Advanced Insights

* Match result margins
* Toss impact on match outcome
* Team performance in different venues/cities
* Boundaries analysis: how runs are distributed (1s, 2s, 4s, 6s)

#### 📉 Trend Analysis

* Year-wise scoring patterns
* Powerplay vs death overs scoring
* Comparison of old teams vs new franchises

---

### 📌 Tools & Technologies

* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Plotly
* **Environment:** Jupyter Notebook

---

### 🚀 Outcomes

* Cleaned and analysis-ready IPL dataset
* 20+ detailed visualizations and statistical summaries
* Ready for predictive modeling (e.g. match outcome prediction, player performance)

---

### 🧠 Skills Demonstrated

* Data wrangling & preprocessing
* Exploratory Data Analysis (EDA)
* Handling missing & inconsistent data
* Grouping, aggregation, merging
* Data visualization using multiple libraries
* Cricket domain insight generation

---

### ✅ Next Steps

* Build interactive dashboards using **Streamlit**
* Train machine learning models for **match prediction**
* Analyze **specific seasons, players, or franchises**



