  NovaRetail+ — Customer Behavior Analysis
Exploratory data analysis project for NovaRetail+, a Latin American e-commerce platform. The goal is to identify which customer behavior factors are most strongly associated with annual revenue generated.

This is a correlational analysis — correlation ≠ causation.


🗂️ Dataset
Single file: novaretail_comportamiento_clientes_2024.csv — 15,000 records, 12 columns covering customer demographics, usage behavior, advertising spend, satisfaction, and annual revenue.

🔬 What Was Done

Load & Explore — loaded the dataset, inspected structure with .info(), .head(), and .describe()
Data Preparation — identified variable types (numerical, binary, categorical); documented assumptions; no major cleaning needed
Visualization — correlation heatmap for all variables; scatterplots for the three most relevant pairs
Correlation Coefficients — Pearson and Spearman for numerical pairs; point-biserial for binary vs. numerical; Cramér's V for categorical associations
Business Findings — five findings with numerical evidence, interpretation, and business implications
Limitations & Next Steps — analysis boundaries and recommended follow-up actions


💡 Key Findings

Monthly purchases have an extremely strong association with annual revenue (Pearson = 0.97) — the dominant signal in the data
Monthly visits show moderate correlation with both purchases (0.35) and annual revenue
Directed ad spend is moderately correlated with visits (0.58) — advertising aligns with traffic but doesn't guarantee conversion
Churn and premium membership show weak correlations with most variables; satisfaction is the only meaningful signal
Device type and region are statistically independent — no need to segment campaigns by this combination


▶️ How to Run
Open in Google Colab: File → Open notebook → GitHub, paste this repo URL, upload the dataset, and run all cells.
Or locally:
bashpip install pandas numpy matplotlib seaborn scipy
jupyter notebook NovaRetail_Analysis.ipynb

Place the CSV file at /datasets/novaretail_comportamiento_clientes_2024.csv relative to your working directory.


👤 Author
Rocio — Data Analytics Student
