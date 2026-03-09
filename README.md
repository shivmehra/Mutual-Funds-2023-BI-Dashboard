# Mutual-Funds-2023-BI-Dashboard
Fund Analysis for the Mutual funds in the market (2000+). Fund analysis by cleaning data and building a data model in Power BI, to create a Dashboard.

DATA SET FROM:  HTTPS://WWW.KAGGLE.COM/DATASETS/ASHISHRAUT64/MUTUAL-FUNDS-INDIA

Creating Derived Columns
I’ll need to create several derived (calculated) columns or measures from my existing columns.
My current columns are:
•	S.no
•	Scheme
•	Category
•	Type
•	Benchmark
•	Rating
•	Net_Asset_Value(Rs.)
•	CAGR% 6 Months
•	CAGR% 1 Year
•	CAGR% 3 Year
•	Min. Invest(Rs.)
•	Exp. Ratio(%)
•	SIP Min. Inv.(Rs.)
Below are the additional columns/measures I should create to start analyses.
•	Performance Score
  o	Purpose:
    	Ranking best funds overall
    	Fund screener page
•	Return Stability
  o	Purpose:
    	Identify consistent performers
    	Lower value = stable performance
•	Momentum
  o	Purpose:
    	Detect funds are gaining momentum recently
•	Return Efficiency
  o	Purpose:
    	Measure the return generated per unit cost
    	Very useful visual:
      Expense vs Return efficiency.
•	Cost Category
  o	Purpose:
    	Cost distribution visuals
    	Cost comparison charts
•	Affordability Score
  o	Purpose:
    	Find high-return funds with a low entry barrier.
•	SIP Friendliness
  o	Purpose:
    	Investor accessibility analysis.
•	Investment Size Category
  o	Purpose:
    	Investment accessibility visuals.
•	NAV Range
  o	Purpose:
    	NAV distribution visuals.
•	Rating Category
  o	Purpose:
    	Rating comparison analysis.
•	Rank by 3Y Return
•	Rank by Expense Ratio
•	Rank by Performance Score
•	Return Variation
  o	Purpose:
    	Approximate return consistency.
    	Lower = stable fund.
•	Performance Category
  o	Purpose:
    	Growth segmentation.

Power BI Dashboard Created:
Page 1 — Dashboard Overview
Purpose: High-level summary of the dataset
KPI Cards (Top Row)
Show quick insights.
•	Total Schemes
•	Average 1Y CAGR
•	Average 3Y CAGR
•	Average Expense Ratio
•	Average NAV
•	Average Minimum Investment
Visuals
1 Category Distribution
•	Chart: Pie / Donut
•	Value: Count of Scheme
•	Legend: Category
Shows market share of fund categories.
________________________________________
2 Top 10 Performing Funds (3-Year CAGR)
Chart: Bar chart
Columns:
•	Scheme
•	CAGR 3 Year
Sort descending.
________________________________________
2 Average Returns by Category
Chart: Clustered bar
X-axis: Category
Y-axis: Avg CAGR 1Y / Avg CAGR 3Y
________________________________________
4 Ratings Distribution
Chart: Column chart
X-axis: Rating
Y-axis: Count of Schemes
________________________________________
Filters (Left Side)
Slicers:
•	Category
•	Type
•	Rating
•	Benchmark
________________________________________
Page 2 — Performance Analysis
Purpose: Deep dive into returns
1 CAGR Comparison
Chart: Clustered bar
Axis: Scheme
Values:
•	CAGR 6M
•	CAGR 1Y
•	CAGR 3Y
________________________________________
2 Return Consistency
Chart: Scatter Plot
X-axis:
CAGR 6M
Y-axis:
CAGR 3Y
Legend:
Category
This shows:
•	short-term outperformers
•	long-term stable funds
________________________________________
3 Top vs Bottom Performers
Two visuals:
Top 10 funds by 3Y CAGR
Bottom 10 funds by 3Y CAGR
________________________________________
4 Category Performance Heatmap
Matrix:
Rows:
Category
Columns:
Return Period
•	6M
•	1Y
•	3Y
Values:
Average CAGR
