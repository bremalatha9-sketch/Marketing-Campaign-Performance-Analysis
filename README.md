# [Project Title]
*Marketing Performnce Campaign Analysis*

## 📖 Table of Contents
- [Project Overview](#-project-overview)
- [Data Source](#-data-source)
- [Tools & Technologies](#-tools--technologies)
- [Data Cleaning & Preparation](#-data-cleaning--preparation)
- [Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
- [Key Insights](#-key-insights)
- [Recommendations](#-recommendations)
- [How to Use](#-how-to-use)

## 📊 Project Overview
This project focuses on analysing marketing campaign performance using Python and Power BI. It helps to understand which campaigns and marketing channels perform better.
The project analyses revenue, cost, ROI, CTR, CPC, clicks, conversions, and customer engagement.
The main goal is to find useful business insights and help businesses make better marketing decisions.

## 🗂️ Data Source
Hugging face data source. The dataset contains 20,000 records and 16 columns.

## 🛠️ Tools & Technologies
- **Language:** Python (Pandas, NumPy, Seaborn) or R
- **Database:** SQL (PostgreSQL/MySQL)
- **Visualization:** Tableau, Power BI, or Matplotlib
- **Documentation:** Jupyter Notebook

## 🧹 Data Cleaning & Preparation
1. Handled Missing Values and Duplicates
- Checked missing values in the dataset.
- Removed duplicate rows.
- Checked duplicate Campaign IDs and kept the first occurrence.
2. Formatted Data Types
- Converted the date column into datetime format.
- Converted numerical columns into numeric format.
- Removed $, commas and the word "days" from values.
- Renamed columns by removing extra spaces and using lowercase letters.
3. Created New Calculated Columns (Feature Engineering)
- Extracted month from the date column for monthly analysis.
- Created new columns where needed for campaign performance analysis.
## 🔍 Exploratory Data Analysis (EDA)
What is the overall spend, revenue, profit and ROI?
- Which channels, campaign types and audiences perform best?
- How do revenue and conversions change by month?
- What drives profit: spend, ROI, clicks, CTR, CPC, conversion?
- Do bigger budgets pay off (cost per conversion)?
- How should CTR/CPC outliers be handled? (capped at the IQR limit, raw values kept)


<img width="946" height="684" alt="Heat map" src="https://github.com/user-attachments/assets/9d89766f-703c-42a2-a8c9-1038b091f09e" />
This is a Correlation Heatmap. It shows the relationship between different campaign performance metrics.

What is it saying? shows whether two metrics have a positive or negative relationship. 
What features you used? acquisition_cost(),revenue(), roi, clicks, conversion Rate,ctc,cpc,profit revenue moves with spend (0.75) and ROI (0.63). CTR, CPC, conversion rate and engagement are near 0.0 with profit, so they don't predict it.

From this what you are showing us? Acquisition Cost and Revenue: 0.75 (Strong positive relationship). ROI and Revenue: 0.63 (Positive relationship). CTR and CPC: -0.48 (Negative relationship). Other metrics show very little correlation. correlation heatmap to analyse the relationship between different campaign performance metrics. Red indicates positive correlation, and blue indicates negative correlation. From this chart, I found that acquisition cost and revenue have a strong positive correlation of 0.75. ROI and revenue also have a positive correlation of 0.63. This helps us understand the relationship between different marketing metrics.


## 💡 Key Insights
Campaign Performance: Social Media campaigns achieved the highest average ROI compared to other campaign types.
Campaign Distribution: All five campaign types had almost equal numbers of campaigns.
Revenue Analysis: Monthly revenue analysis helps identify changes in campaign revenue over time.
Channel Performance: Different marketing channels showed differences in CTR and conversion rates.
Customer Engagement: Engagement levels were slightly different across campaign types.

## 🚀 Recommendations
Don't move budget between channels; their ROI is within 0.1x.
Focus more on campaign types that generate higher ROI.
Improve marketing strategies for low-performing channels.
Monitor monthly revenue to identify performance changes.
Improve customer engagement to increase conversions.
Compare marketing costs and revenue before allocating campaign budgets.
## ⚙️ How to Use
Explain how someone else can run your project.
- List dependencies (e.g., `pip install -r requirements.txt`).
- Provide instructions for running the notebook or script.

