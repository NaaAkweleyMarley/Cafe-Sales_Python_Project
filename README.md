# Café Sales Report
### Descriptive, diagnostic, predictive and prescriptive analytics of café sales

#### About the Project

**Café Sales Report** is a Python-based data analysis project that explores sales performance from the Café Sales dataset. The data was cleaned and visualised in Python to uncover trends in:

- Quantity purchased
- Revenue generated
- Payment methods
- Product performance

The analysis moves through descriptive and diagnostic analytics, to predictive analytics and prescriptive analysis, and ends with a conclusion and recommended business actions.

It is an analytical and data visualisation exercise intended to demonstrate how transaction data can be transformed into meaningful insights. The results should be interpreted in the context of the project rather than as independently verified business results.

#### Project Objectives

The analysis was carried out to explore five main objectives:

1. Analyze total sales over time (daily, weekly, or monthly).
2. Identify the best-selling items by quantity and total revenue.
3. Compare total sales across different product categories (e.g., Coffee, Pastry, Drinks).
4. Determine the most popular payment methods (e.g., Cash, Card, Mobile).
5. Identify the factors that significantly affect total revenue.


#### Project Components

##### 1. Data Cleaning

The following steps were taken to prepare the data:

1. Filled missing numeric values with the mean.
2. Replaced invalid entries like "ERROR", "UNKNOWN" and NaN with appropriate values ('Unspecified').
3. Ensured all dates were in a consistent format.
4. Feature Engineering: Created new columns, such as Day of the Week or Transaction Month, for further analysis.
5. Standardized and crosschecked data types for all columns.

##### 2. Objective 1: Total Sales Over Time

The bar chart with a trendline shows total sales for each month from January to December:

- Jan — 7,212.51
- Feb — 6,637.51
- Mar — 7,171.93
- Apr — 7,156.99
- May — 6,933.89
- Jun — 7,376.49
- Jul — 6,894.11
- Aug — 7,063.79
- Sep — 6,848.08
- Oct — 7,304.41
- Nov — 6,985.54
- Dec — 7,172.11

Sales was highest in the month of June. There was a similar spike in sales from September to October.

##### 3. Objective 2: Best-Selling Items by Quantity and Total Revenue

Two bar charts show the top five items.

**Top 5 Items by Quantity Purchased:**

- Coffee — 3,367
- Juice — 3,306
- Salad — 3,263
- Cake — 3,233
- Sandwich — 3,207

**Top 5 Items by Total Revenue:**

- Salad — 16,128.61
- Sandwich — 12,827.71
- Smoothie — 12,583.92
- Juice — 9,999.00
- Cake — 9,786.59

Coffee and Salad were the best-selling items per Quantity and Total Revenue respectively.

##### 4. Objective 3: Comparing Total Sales Across Different Product Categories

The horizontal bar chart shows total revenue per item:

- Salad — 16,128.61
- Sandwich — 12,827.71
- Smoothie — 12,583.92
- Juice — 9,999.00
- Cake — 9,786.59
- Unspecified — 8,140.85
- Coffee — 6,953.70
- Tea — 4,933.46
- Cookie — 3,403.52

Salad generated the highest revenue ($16,128.61), followed by Sandwich and Smoothie, meaning that these products drive the most income for the business.

##### 5. Objective 4: Most Popular Payment Methods

The pie chart shows sales by payment method:

- Unspecified — 31.0%
- Digital Wallet — 23.1%
- Cash — 23.0%
- Credit Card — 22.8%

Sales payments were made through four channels as indicated in the pie chart, with usage patterns nearly equal and Digital Wallet barely leading. There was, however, a large portion of transactions that did not specify the method, accounting for 31% of the data.

##### 6. Objective 5: Factors That Significantly Affect Total Revenue

The correlation matrix compares Total Spent, Quantity, Item Count and Price Per Unit:

| | Total Spent | Quantity | Item Count | Price Per Unit |
|---|---|---|---|---|
| **Total Spent** | 1 | 0.7 | 0.12 | 0.65 |
| **Quantity** | 0.7 | 1 | 0.0029 | 0.0039 |
| **Item Count** | 0.12 | 0.0029 | 1 | 0.19 |
| **Price Per Unit** | 0.65 | 0.0039 | 0.19 | 1 |

The correlation matrix shows a strong positive relationship (0.7) between Total Spent and Quantity, and between Total Spent and Price Per Unit (0.65). This suggests that both higher prices and higher purchase volumes contribute significantly to total revenue.

##### 7. Predictive Analytics

- **Goal:** Predict how much a customer will spend.
- **Method:** Linear Regression, using Item, Payment Method and Location as predictors.

The actual vs. predicted scatter plot shows predicted values closely following actual values across the range, consistent with the model's R² of 0.90.

The evaluation metrics obtained were:

- **R2 Score:** 0.9025263741052887
- **Mean Abs Error:** 1.3303245720684742
- **Mean squared error:** 3.265795030061989

These metrics confirm that the forecasts from the model are reliable.

##### 8. Prescriptive Analysis (Recommended Business Actions)

1. Promote high-revenue items like Salad, Sandwich and Smoothie to increase revenue.
2. Improve stock management by ensuring consistent availability of top-performing products.
3. Bundle best-selling with low-revenue items (e.g., Coffee and Cookie) to increase sales.
4. Introduce loyalty discounts for high-frequency buyers.
5. Optimize pricing: slightly reduce prices on low-selling items to attract more customers.

#### Key Insights

The analysis provides several initial observations that can guide further decisions.

##### a. Sales Over Time

Sales was highest in the month of June, and there was a similar spike in sales from September to October.

##### b. Best-Selling Items

Coffee and Salad were the best-selling items per Quantity and Total Revenue respectively.

##### c. Revenue Drivers

Salad, Sandwich and Smoothie are the café's main revenue drivers, generating the most income for the business.

##### d. Payment Methods

Usage across payment methods is nearly equal, with Digital Wallet barely leading. A large portion of transactions (31%) did not specify the method.

##### e. Factors Affecting Revenue

Both higher prices and higher purchase volumes contribute significantly to total revenue.

##### f. Predictive Model

The predictive model estimates customer spend reliably, with an R² of 0.90.

These observations are descriptive findings from the analysis. They do not, on their own, establish the causes of differences in sales or explain the underlying business conditions.

#### Conclusion

This analysis shows that Salad, Sandwich and Smoothie are the café's main revenue drivers, with demand peaking from September to October. The predictive model estimates customer spend reliably, and if current patterns continue, sales should remain steady. By promoting top earners, bundling popular items and keeping key products in stock, the café can turn these insights into better decisions.

#### Tools Used

- **Python** — Data cleaning, Data visualisation and Predictive modelling.
- **Linear Regression** — Predicting customer spend.
- **JupyterLab** — Analysis environment.

#### Visualisations

The analysis uses a combination of:

- Bar chart with trendline
- Bar charts
- Horizontal bar chart
- Pie chart
- Correlation matrix
- Scatter plot (actual vs. predicted)

#### Project Workflow

The analysis follows these stages:

##### i. Data Cleaning

Clean the data, standardise dates and data types, and create new features.

##### ii. Descriptive and Diagnostic Analytics

Explore total sales over time, best-selling items, revenue by item, payment methods and the factors affecting total revenue.

##### iii. Predictive Analytics

Use Linear Regression to predict how much a customer will spend.

##### iv. Prescriptive Analysis

Turn the findings into recommended business actions.

#### Presentation

The full findings are summarised in the accompanying slide deck: [Cafe-Sales_Presentation.pdf]

The dataset used in the analysis is included as [Cafe-Sales_dataset.csv]


#### Project Summary
This repository delivers an end-to-end analytical framework designed to evaluate multi-dimensional café performance. By engineering a structured diagnostic workflow, the project allows for fluid exploration across key retail dimensions, including temporal sales trends, item-level revenue distributions, payment method utilization, and underlying revenue drivers.

The project highlights the technical integration of a full data pipeline, moving from rigorous data cleaning and feature engineering to exploratory data analysis (EDA) and predictive modeling, to build a reliable decision-support system which can be adopted by retail environments.

#### Author:
#### Naa Akweley Marley
LinkedIn: [Naa Akweley Marley](https://www.linkedin.com/in/naa-akweley-marley)