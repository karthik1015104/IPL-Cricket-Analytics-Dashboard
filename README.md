# IPL Match Analytics

An end-to-end exploratory data analysis project on Indian Premier League (IPL) cricket data, uncovering team performance trends, batting and bowling insights, venue patterns, and match scoring behaviour using Python.

---

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Key Analyses](#key-analyses)
- [Key Findings](#key-findings)
- [Tech Stack](#tech-stack)
- [Setup & Usage](#setup--usage)
- [Dashboard Preview](#dashboard-preview)
- [Author](#author)

---

## Overview

This project analyzes IPL match and ball-by-ball delivery data to answer questions like:
- Which teams have been the most dominant across IPL seasons?
- Does winning the toss actually help you win the match?
- Who are the best batsmen and bowlers in IPL history?
- How do scoring patterns differ between powerplay and death overs?

---

## Dataset

| File | Description | Size |
|------|-------------|------|
| `matches.csv` | Match-level data — teams, venue, toss, result, winner | ~950 matches |
| `deliveries.csv` | Ball-by-ball data — batsman, bowler, runs, wickets, extras | ~179,000 deliveries |

> **Source:** [IPL Complete Dataset on Kaggle](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020)  
> Data covers IPL seasons from **2008 to 2020**.

---

## Project Structure

```
IPL-Match-Analytics/
├── data/
│   ├── matches.csv
│   └── deliveries.csv
├── notebooks/
│   └── IPL_Match_Analytics.ipynb
├── outputs/
│   ├── ipl_dashboard.png
│   ├── team_analysis.png
│   ├── batting_analysis.png
│   └── bowling_analysis.png
├── requirements.txt
├── .gitignore
└── README.md
```

---

## Key Analyses

- **Team Performance** — Total wins and win percentage per team, accounting for matches played
- **Toss Impact** — Whether toss winners have a statistically meaningful advantage
- **Top Batsmen** — All-time run scorers and best strike rates (min. 1000 runs filter)
- **Top Bowlers** — Best economy rates (min. 600 balls) and highest wicket takers
- **Venue Analysis** — Stadiums that have hosted the most IPL matches
- **Runs Distribution** — Histogram of total runs scored per match
- **Powerplay vs Death Overs** — Average runs per ball comparison across match phases

---

## Key Findings

- **Mumbai Indians** lead all-time IPL wins across seasons
- Toss winners go on to win the match roughly **50–52%** of the time — barely better than a coin flip
- **Virat Kohli** tops the all-time run-scoring charts
- Death overs produce significantly more runs per ball than powerplay overs
- **Wankhede Stadium** and **Eden Gardens** are the most frequently used venues

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3 | Core language |
| Pandas | Data loading, cleaning, aggregation |
| NumPy | Numerical operations |
| Matplotlib | All visualizations and dashboard |
| Seaborn | Plot styling |
| Jupyter Notebook | Development environment |

---

## Setup & Usage

**1. Clone the repository**
```bash
git clone https://github.com/yourusername/IPL-Match-Analytics.git
cd IPL-Match-Analytics
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Add the dataset**

Download `matches.csv` and `deliveries.csv` from [Kaggle](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020) and place them inside the `data/` folder.

**4. Run the notebook**
```bash
jupyter notebook notebooks/IPL_Match_Analytics.ipynb
```

Or open directly in [Google Colab](https://colab.research.google.com/).

---

## Dashboard Preview

![IPL Dashboard](outputs/ipl_dashboard.png)

---

## Author

**Karthik**  
[GitHub](https://github.com/yourusername) • [LinkedIn](https://linkedin.com/in/yourusername)
