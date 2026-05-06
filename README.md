# Subscription Data Audit Project

## Project Description
This project involves a comprehensive audit of subscription application data. The primary goals are to identify opportunities for cost savings, improve customer satisfaction, and ensure data accuracy. 

Key aspects include:
*   **Identifying potential savings**: By analyzing monthly fees and negotiation success probabilities.
*   **Prioritizing negotiation efforts**: Categorizing subscriptions into priority tiers.
*   **Understanding user sentiment**: Categorizing user feedback to address issues like 'Churn Risk' or 'Pricing Complaint'.
*   **Detecting anomalies and errors**: Flagging outliers and data quality issues.
*   **Cleaning and standardizing data**: Ensuring consistent and reliable data for analysis.

Ultimately, it aims to provide actionable insights to optimize subscription costs and enhance the overall user experience.

## Installation
To run this project, you will need to have Python and the following libraries installed:

```bash
pip install pandas openpyxl matplotlib seaborn scipy
```

## Usage
1.  **Place your data**: Ensure your raw subscription data is in an Excel file named `raw_app_data_audit.xlsx` in the same directory as the notebook, or update the `file_path` variable in the first code cell.
2.  **Run the notebook**: Execute all cells in the Jupyter notebook or Google Colab environment.
3.  **Review Outputs**: The notebook will generate several output files and visualizations:
    *   `processed_app_data_audit.xlsx`: The cleaned and processed DataFrame.
    *   `final_clean_audit_master.csv`: The master cleaned data in CSV format.
    *   `human_audit_priority_list.csv`: A list of transactions flagged for manual review (outliers or missing dates).
    *   `executive_roi_summary.csv`: A summary of ROI by subscription type.
    *   `strategic_priority_targets.csv`: Top 20% of transactions for negotiation focus.
    *   `sentiment_financial_impact.csv`: Pivot table showing sentiment vs. priority.
    *   `FINAL_AUDIT_REPORT_SUMMARY.txt`: A text file summarizing key findings.
    *   Various `.png` image files for charts and visualizations (e.g., `pareto_analysis.png`, `fee_outliers_boxplot.png`, `opportunity_heatmap.png`, `roi_data_integrity.png`, etc.).
    *   `EXECUTIVE_SUMMARY_REPORT.txt`: A final executive summary report.

## Analysis Summary
*   **Total Transactions Processed**: 10,000
*   **Total Expected Savings**: $148,595.41
*   **Data Integrity (Verified Data)**: 75.0%
*   **Anomalies Detected (Requires Human Audit)**: 1,044
*   **Date Accuracy (Valid Dates)**: 75.8%
*   **Top Opportunity**: netflix (highest expected savings)
*   **Top Sentiment Risk**: General Inquiry (most frequent user feedback category)
*   **Pareto Principle**: The top 20% of transactions account for approximately 91.2% of the total potential savings.
