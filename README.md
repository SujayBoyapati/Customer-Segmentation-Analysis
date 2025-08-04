# Customer-Segmentation-Analysis

OBJECTIVE: 
Segmentation of mall customers into distinct groups based on Age, Annual Income, and Spending Score using rule-based logic to stimulate business logic and descision-making rather than clustering algorithms.

TOOLS:
- VS CODE
- Jupyter Notebook(via VS CODE)
- Python
  - Pandas
  - Seaborn
  - Matplotlib
- SQLite(SQL Queries)
- GitHub(Version Control)

DATASET:
File: Mall_Customers.csv
Columns: 
- CustomerID: Unique ID for each customer
- Gender: Male / Female
- Age: Age of the customer
- Annual Income (k$): Income in thousands of dollars
- Spending Score (1-100): Score assigned based on customer behavior


DATA CLEANING:
Removed duplicates and null values (if any)
Converted Gender to numeric:
- 0 = Male
- 1 = Female

Verified correct data types for each column


SEGMENTATION:
Customers are segmented into groups based on business-defined logic:
➤ Age Groups
- 18–30 → Youth
- 31–45 → Middle-Aged
- 46+ → Senior
  
➤ Income Groups
- 0 ≤ 40k → Low-Income
- 41–65k → Medium-Income
- 65k → High-Income
  
➤ Spending Groups
- 0–40 → Low Spending
- 41–65 → Medium Spending
- 66–100 → High Spending
(Final Segment Label: "Age Group | Income Group | Spending Group")


SQL ANALYSIS: 
Data was loaded into a SQLite database using the sqlite3 module in VS Code for analysis and integration with Pandas. The following queries were performed:
- Total number of customers
- Average age, income, and spending score
- Average income/spending by gender
- Count of customers in each age/income/spending bracket

DATA ANALYSIS(EDA)
Implemented Exploratory Data Analysis using Seaborn and Matplotlib to perform visualize behaviors and relationships between groups
Histograms & Box Plots
- Distribution of Age
- Distribution of Annual Income
- Distribution of Spending Score
Pair Plot
- Visual correlation between Age, Income, and Spending Score

INSIGHTS
- High distribution of Youth and Middle-Income groups as they show a wider range of spending behaviors
- Drastic spread among spending scores and high-income across all age groups


