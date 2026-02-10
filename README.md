Taiwan Bankruptcy Financial Ratio Analysis

A Python-based exploratory data analysis (EDA) project comparing bankrupt and non-bankrupt companies using key financial ratios from the Taiwan Bankruptcy Prediction dataset.

This project focuses on identifying financial patterns associated with corporate failure through descriptive statistics and visual analysis.

Overview

The objective of this project is to analyze and compare financial health indicators between bankrupt and healthy firms.
It provides insights that can support bankruptcy prediction, financial risk assessment, and feature selection for machine learning models.

Dataset

Dataset: Taiwan Bankruptcy Prediction

Target Column: Bankrupt?

0 → Non-Bankrupt

1 → Bankrupt

Features: Financial ratios derived from corporate financial statements

Note: Financial ratios may contain extreme values and skewed distributions.

Financial Ratios Analyzed

ROA (C) before interest and depreciation

Net Income to Total Assets

Liability to Equity

Interest Coverage Ratio (Interest expense to EBIT)

These ratios capture profitability, leverage, and debt-servicing ability, which are critical indicators of financial distress.

Tech Stack

Python 3

pandas

numpy

matplotlib

Recommended environment: Google Colab or Jupyter Notebook.

Analysis Steps

Load and clean the dataset

Inspect data structure and missing values

Split data into bankrupt and non-bankrupt groups

Compute group-wise averages and percentage differences

Visualize distributions using boxplots

Compare mean values using bar charts

Generate summary statistics

Visualizations

Boxplots comparing financial ratio distributions

Bar charts showing average ratio differences

Tabular summaries of means and standard deviations

Key Findings

Bankrupt firms show significantly lower profitability.

Leverage ratios are notably higher among bankrupt companies.

Interest coverage is substantially weaker for bankrupt firms.

Overlapping distributions indicate the need for multivariate or machine-learning-based models.

Future Improvements

Statistical significance testing (t-test, Mann–Whitney U)

Effect size calculation (Cohen’s d)

Outlier treatment (winsorization)

Machine learning models for bankruptcy prediction

Comparison with classical models (e.g., Altman Z-Score)

How to Run
pip install pandas numpy matplotlib


Update the dataset path if needed:

df = pd.read_csv("path/to/taiwan_bankruptcy.csv")


Run all cells to reproduce the analysis and visualizations.

Use Cases

Academic research and thesis work

Financial risk analysis

Feature exploration for machine learning models

Educational demonstrations

License

This project is for educational and research purposes.
