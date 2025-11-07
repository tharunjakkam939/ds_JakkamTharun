# 🧠 Data Science Assignment – Web3 Trading Team  
**Author:** Tharun Jakkam  
**Repository:** `ds_Tharun`  
**Platform:** Google Colab + Python  

---

## 📌 Objective
Analyze the relationship between trader behavior and overall market sentiment using on-chain trade data and the *Fear & Greed Index*.  
The analysis explores how metrics like **PnL**, **trade frequency**, **notional size**, and **win rate** vary during different sentiment phases (Extreme Fear → Extreme Greed).

---

## 📂 Project Structure
ds_Tharun/
├── data/
│ ├── trades.csv
│ └── fear_greed.csv
│
├── csv_files/
│ ├── merged_daily.csv
│ └── final_output.csv
│
├── outputs/
│ ├── pnl_trend.png
│ ├── pnl_by_sentiment.png
│ └── correlation_heatmap.png
│
├── notebook_1.ipynb
└── ds_report.pdf


---

## ⚙️ Setup & Execution (Google Colab)
1. **Open the Notebook:**  
   Upload or open `notebook_1.ipynb` in **Google Colab**.

2. **Mount Google Drive:**
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
Ensure Folder Structure Exists:

My Drive/
└── ds_Tharun/
    └── data/
        ├── trades.csv
        └── fear_greed.csv


Run All Cells Sequentially:
The notebook automatically:

Loads and cleans both datasets

Aggregates daily trade metrics

Merges with Fear & Greed index

Performs EDA and visualization

Runs t-tests and ML model

Exports processed files and plots

📊 Outputs Overview
Type	File	Description
CSV	merged_daily.csv	Cleaned & merged daily dataset
CSV	final_output.csv	Final processed data for reporting
PNG	pnl_trend.png	Daily PnL trend visualization
PNG	pnl_by_sentiment.png	PnL distribution across sentiment levels
PNG	correlation_heatmap.png	Feature correlation visualization
PDF	ds_report.pdf	Final analytical summary report
🧮 Methodology Summary

Data Cleaning & Preparation: Standardized column names, handled missing timestamps, and derived trade dates.

Feature Engineering: Computed metrics — total PnL, average execution price, win rate, and notional values.

Merging: Combined trader and sentiment data by date.

Visualization: Trend plots, boxplots, and correlation heatmaps.

Statistical Analysis: t-test comparison for Fear vs Greed performance.

Predictive Modeling: Random Forest classifier predicting profitable vs non-profitable days.

📈 Key Insights

Trader performance improves significantly during Greed sentiment phases.

Extreme Fear correlates with lower activity and profitability.

PnL shows a positive correlation with sentiment value.

The model achieved ≈ 80% accuracy in predicting profitable days.

Emotional market phases visibly influence trader decisions.

🧠 Tools & Libraries
Category	Libraries Used
Data Handling	pandas, numpy
Visualization	matplotlib, seaborn
Statistical Analysis	scipy.stats
Machine Learning	scikit-learn
Environment	Google Colab, Google Drive
📘 Report Summary

All findings, visuals, and methodology explanations are documented in ds_report.pdf.
It includes:

Objective & Dataset Overview

Methodology

Visual Analysis

Statistical Findings

Predictive Insights

Conclusion & Future Work

🔗 Links

Google Colab Notebook: Open in Colab
 ← (Add your public Colab link here)

GitHub Repository: https://github.com/yourusername/ds_Tharun

🏁 Conclusion

This analysis demonstrates a clear correlation between market sentiment and trader performance.
Periods of Greed show higher profitability and trading confidence, whereas Fear phases correspond to conservative behavior and lower gains.
By combining sentiment analysis with behavioral data, the model highlights how psychological factors shape real-world trading dynamics.
