# Sales Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Tools](#tools)
- [Data Analysis](#data-analysis)
- [Recommendations](#recommendations)

### Project Overview

This data analysis project delves into the sales performance of an e-commerce company across 2021 and 2022. Our goal is to uncover trends, offer data-driven recommendations, and achieve a comprehensive grasp of the company's performance by scrutinizing different facets of the sales data. This includes examining factors such as product sales patterns, sales types, seasonal variations, and payment modes to extract actionable insights and improve strategic decision-making processes.

### Data Sources

The dataset utilized for this analysis is the "sales_data.csv" file, which comprises comprehensive details regarding every sale conducted by the company.

### Tools
- Excel - Data Cleaning  [Download here](https://www.microsoft.com/en-us/microsoft-365/download-office)
- Python - Data Cleaning  [Download here](https://www.anaconda.com/download)
- SQL Server - Data Analysis [Download here](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
- PowerBI - Creating reports  [Download here](https://powerbi.microsoft.com/en-us/downloads/)

### Data cleaning/ Preparation
In the initial data preparation phase, we performed the following tasks:

1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formatting.

### Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions, such as:

- What is the overall sales trend?
- Which products are top sellers?
- What are the peak sales periods?

### Data Analysis
Features worked with:

1. SQL
```sql
-- Selecting with a condition
SELECT * FROM Sales
WHERE cond = 2;
```

2. Python
```python
# Transposing data
import pandas as pd

# Replace 'input.csv' with the path to your CSV file
input_file = r'C:\Users\ian.muthengi\Downloads\Sales.xlsx'

# Read the CSV file into a pandas DataFrame
df = pd.read_excel(input_file)

# Transpose the DataFrame
df_transposed = df.transpose()

# Replace 'output_transposed.csv' with the desired output file name
output_file = 'C:/Users/ian.muthengi/Downloads/transposed_sales.xlsx'

# Write the transposed DataFrame to a new CSV file
df_transposed.to_excel(output_file, index=True, header=False)
```
3. Power BI

### Results/Findings
The analysis results are summarized as follows:

1. The company's sales have been steadily increasing as from 2021 to 2022, with a noticeable peak during the holiday season.
2. Product41 is the best-performing category in terms of sales.
3. Direct sales account for the highest percentage in terms of sales type.

### Recommendations
Based on the analysis, we recommend the following actions:

1. Invest in marketing and promotions during peak sales seasons to maximize revenue.
2. Focus on expanding and promoting products41.
3. Emphasize expanding and promoting direct sales.

### Limitations
I had to remove all zero values from buying price and selling price columns because they would have affected the accuracy of my conclusions from the analysis. There are still a few outliers even after the omissions but even then we can still see that there is a positive correlation between both buying price and number of votes with selling price.
