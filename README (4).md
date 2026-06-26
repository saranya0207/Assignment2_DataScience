# Factors Influencing Global Happiness: An Exploratory Data Analysis of the World Happiness Report (2011–2025)
<img width="1000" height="350" alt="image" src="https://github.com/user-attachments/assets/0ca5d56b-fc2c-4716-9306-25f593909dd8" />

---
## 📌 Overview

This project analyses the World Happiness Report dataset, covering 168 countries across 14 survey years (2011–2025). It demonstrates data cleaning, exploratory data analysis (EDA), visualization, and insight generation using a real-world, open-source panel dataset with inherent data quality challenges. The notebook is designed to communicate actionable insights to stakeholders through clear, evidence-based visualizations and interpretations.

## 🎯 Problem Statement

1. Which countries are consistently the happiest / least happy in the world?
2. How has Malaysia's happiness ranking changed over 15 years compared to ASEAN neighbours?
3. Which socio-economic factor contributes most to explaining life evaluation scores globally?
4. Does GDP per capita reliably predict happiness?
5. How has global average happiness trended over time, and was there a measurable COVID-19 effect?

## 🗂️ Repository Structure

```
.
├── README.md                              # This file
├── WHR_Analysis.ipynb                     # Main analysis notebook (Colab-ready)
└── WHR_Data.xlsx                          # Raw dataset
```

## 📊 Dataset

- **Source:** World Happiness Report 2026
- **Link:** https://worldhappiness.report/data-sharing/
- **Size:** 2,116 rows × 13 relevant columns
- **Period:** 2011–2025

## 📈 Visualizations Included

1. Top/bottom 10 happiest countries (2025)
2. Malaysia vs ASEAN happiness trends (2011–2025)
3. Distribution of factor contributions (2019–2025)
4. GDP per capita vs life evaluation
5. Global average happiness over time with COVID-19 annotation
6. Correlation heatmap of all explanatory factors
   
## 🔑 Key Findings

- Nordic countries consistently ranked as the happiest, while conflict-affected countries recorded the lowest life evaluation scores.

- Malaysia showed gradual post-pandemic recovery and remained a moderately happy country within ASEAN.

- Log GDP per capita, Healthy Life Expectancy, and Social Support were the factors most strongly associated with life evaluation.

- Higher GDP contribution was associated with greater happiness, although social and institutional factors also influenced life evaluation.

- Global average happiness remained relatively stable, with a modest decline during the COVID-19 period followed by gradual recovery.


## ▶️ How to Run

1. Open `WHR_Analysis.ipynb` in Google Colab.
2. Upload `WHR_Data.xlsx` to the Colab session (or place it in the Drive folder and mount it).
3. Run all cells top to bottom.

**Dependencies:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `openpyxl`.
