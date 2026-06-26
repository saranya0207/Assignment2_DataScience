# 🌍 World Happiness Report 2026 — Global Wellbeing Analysis (2011–2025)

**STQD6014 — Project 2 (25%)**
Master of Science (Data Science and Analytics)

## 📌 Overview

This project analyses the **World Happiness Report 2026** dataset (Figure 2.1), covering **168 countries across 14 survey years (2011–2025)**. It demonstrates data cleaning, exploratory visualization, and insight generation on a real, "dirty" open-source panel dataset, structured as a stakeholder-facing analytical notebook.

## 🎯 Problem Statement

1. Which countries are consistently the happiest / least happy in the world, and how has the gap evolved?
2. How has Malaysia's happiness ranking changed over 15 years compared to ASEAN neighbours?
3. Which socio-economic factor contributes most to explaining life evaluation scores globally?
4. Does GDP per capita reliably predict happiness — where does the relationship break down?
5. How has global average happiness trended over time, and was there a measurable COVID-19 effect?

## 🗂️ Repository Structure

```
.
├── README.md                              # This file
├── WHR2026_Happiness_Analysis.ipynb       # Main analysis notebook (Colab-ready)
└── WHR26_Data_Figure_2_1.xlsx             # Raw dataset
```

## 📊 Dataset

- **Source:** World Happiness Report 2026, Figure 2.1
- **Link:** https://worldhappiness.report/data-sharing/
- **Size:** 2,116 rows × 13 relevant columns
- **Period:** 2011–2025 (2013 not published)
- **Key fields:** Life Evaluation (Cantril Ladder), Rank, and six explanatory factors (GDP per capita, social support, healthy life expectancy, freedom, generosity, corruption perception)

## 🧹 Data Cleaning Summary

| Issue | Resolution |
|---|---|
| 15 redundant blank columns | Dropped |
| Inconsistent column names | Standardised to snake_case |
| Non-ASCII / inconsistent country names | Mapped to common English names |
| Structural missingness in explanatory factors (2011–2018) | Preserved; separate `df_factors` (2019–2025) subset created instead of imputing |
| Duplicates / out-of-range values | Checked — none found |

## 📈 Visualizations Included

1. Top/bottom 10 happiest countries (2025) — bar chart
2. Malaysia vs ASEAN happiness trends (2011–2025) — line chart
3. Distribution of factor contributions (2019–2025) — box plot
4. GDP per capita vs life evaluation — scatter plot with regression
5. Global average happiness over time with COVID-19 annotation — line chart
6. Correlation heatmap of all explanatory factors

Each chart is paired with a written insight supported by published WHR findings and external sources (full references in the notebook).

## 🔑 Key Findings

- Nordic/high-trust countries (Finland, Iceland, Denmark) dominate the top rankings; conflict-affected states anchor the bottom.
- Malaysia shows a gradual post-pandemic recovery (5.34 → 6.01) and ranks mid-table within ASEAN.
- GDP per capita, healthy life expectancy, and social support are the strongest drivers of happiness; generosity plays a minor role.
- The GDP–happiness relationship is positive but non-linear (diminishing returns beyond a threshold).
- Global average happiness dipped only modestly during COVID-19 (2019–2021) and has since recovered.

## ▶️ How to Run

1. Open `WHR2026_Happiness_Analysis.ipynb` in Google Colab.
2. Upload `WHR26_Data_Figure_2_1.xlsx` to the Colab session (or place it in the same Drive folder).
3. Run all cells top to bottom — no additional configuration required.

**Dependencies:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `openpyxl` (all pre-installed in Colab).

## 📚 References

- Helliwell, J. F., Layard, R., Sachs, J. D., De Neve, J.-E., Aknin, L. B., & Wang, S. (Eds.). *World Happiness Report* (2022–2024). Sustainable Development Solutions Network.
- World Bank. (2023). *East Asia and Pacific Economic Update*. World Bank Group.
- World Happiness Report. (2026). *Data for Figure 2.1*. https://worldhappiness.report/data-sharing/

---
*Submitted as part of STQD6014 Project 2, Semester 2 2025/2026.*
