
# Banking System

#### Dashbord link - https://app.powerbi.com/groups/me/reports/63b83fb5-e5ea-4d32-aa65-2693b8714d0f/7f65feb570312a45ea04?experience=power-bi

In today's highly competitive financial environment, understanding customer behavior and financial health is critical for banks to improve services, reduce risk, and increase profitability. This project aims to analyze banking data to identify key factors that influence customer product holdings, credit usage, income levels, and overall engagement with the bank.

The goal is to:

- Uncover trends and patterns in customer demographics, credit card usage, loan amounts, and savings.

- Segment customers based on their financial behavior.

- Identify high-value customers for cross-selling opportunities.

- Predict potential loan default risks or high credit card balances.

- Recommend strategies to improve customer retention and revenue generation.


### Python Analysis
1. Data Upload:
      Uploaded the raw banking data into a MySQL database for structured storage and easy querying.

2. Data Retrieval:
     Retrieved the dataset from MySQL into Python using appropriate SQL queries and connectors for further analysis.

3. Feature Engineering:

     Created new variables such as:

     Age Range (e.g.'17-26', '26-35', '35-43' etc.)

    Income Bins (e.g., low, medium, high)
    
    These new features were used to group and compare customers more effectively.

4. Data Transformation:

    Converted several numerical columns into categorical variables (e.g.'BRId', 'GenderId','IAId','Location ID').

5. Descriptive Statistics

    Computed summary statistics (min, max, median) for key numeric variables like income and lending.
  
    Checked for missing or null values in newly created age bins.

6. Univariate Analysis

    Count plots for categorical variables such as Income Band, Loyalty Classification, Nationality, Fee Structure, etc.
  
    Observed distribution patterns and identified dominant categories (e.g., majority in Low income band).

7. Bivariate Analysis

    Count plots segmented by Gender and Amount of Credit Cards to explore differences in customer profiles.
  
    Analyzed how banking relationships and nationality vary across gender and credit card ownership.

8. Visualizing Lending and Income Patterns

    Bar chart showing median business lending amount by age range band.
  
    Bar chart illustrating income range spread within each age group.

9. Correlation & Relationship Exploration (Visual)

    Explored relationships between income, savings, lending, and categorical customer features via grouped statistics and charts.

10. Distribution Visualization

    Histograms and count plots for all major categorical variables to understand their frequency distributions.



### Power BI Dashboard
The banking data has been visualized through an interactive Power BI dashboard with four key pages to provide actionable insights. These pages are designed for both executive overviews and deep dives into lending and deposit behaviors.

1️. Home Page
  A high-level summary of the bank's customer base and overall financial metrics:

KPIs Displayed:

- Total Number of Customers

- Overall Lending Amount

- Total Superannuation Savings

Total Deposits

2️. Lending Analysis
  Detailed view of the bank’s lending products, with dynamic filtering options:

Slicers:

- Gender

- Banking Relationship 

Metrics:

- Total Bank Loans

- Total Business Lending

- Total Credit Card Balance

Visualizations:

- Total Business Lending by Nationality

- Credit Card Balance by Age Group

- Bank Loans by Occupation

3. Deposit Analysis
  Focuses on deposit products, savings behavior, and account balances:

Slicers:
- Gender
- Banking Relationship

Metrics:

- Total Bank Deposits

- Total Checking Accounts

- Total Foreign Currency Balance

Visualizations:

- Bank Deposits by Occupation

- Foreign Currency Balances by Nationality

- Checking Deposits by Banking Relationship

4️. Summary Page
  Combines lending and deposit insights for a holistic customer overview:

Slicers:

- Gender

- Loyalty Classification

Visualizations:

- Bank Loans & Deposits by Banking Relationship

- Total Loans & Deposits by Nationality

- Total Properties Owned by Customers

- Customer Count by Loyalty Classification

## EDA Insights
1. The chart "Median Business Lending by Age" indicates that, despite the different age groups, the median business loans 
received are relatively consistent across all categories. This suggests that age may not significantly impact access to 
business lending. The uniform distribution of lending amounts implies that lenders are providing equal opportunities to 
entrepreneurs, regardless of their age. Additionally, this could reflect a broader trend of inclusivity in the lending market. 

2. Income range by age range plot shows that income levels are fairly similar across different age groups, indicating that age doesn't have a big impact on income in this case. The bars are about the same height, which suggests that people of various ages earn similar amounts.

3. It shows that the "Low" income band has the highest count, indicating that most people fall into this category. The "Medium" income band is moderate, while the "High" and "Very High" bands are much lower, with "Very High" being minimal. This unequal distribution highlights that many individuals struggle with lower incomes, reflecting broader economic challenges.

4. The count plot for "Banking Relationship" by gender reveals that the "Private Bank" category has the highest count, indicating strong engagement among individuals with private banking services. The "Retail" category follows closely, while the "Institutional" and "Commercial" categories show lower counts, suggesting less representation in these banking relationships. Notably, male and female counts are almost equal across all categories, indicating a balanced gender representation in banking services. This distribution highlights preferences for different types of banking relationships and suggests that both genders are equally engaged.
Nationality

5. The count plot for "Nationality" by gender reveals that the "European" category has the highest count, indicating a significant presence of individuals identifying as European. The "American" and "Asian" nationalities also show notable counts, while the "Australian" and "African" categories have the lowest representation.

6. It reveals that individuals identifying as "European" have the highest number of credit cards, followed by those identifying as "American." In contrast, the counts for "Asian," "Australian," and "African" nationalities are significantly lower, indicating that credit card ownership is more prevalent among Europeans and Americans.

7. It illustrates that most individuals own either one or two properties, with a notable decrease in the count for those owning three properties. This suggests that fewer property holdings are associated with credit card ownership in this dataset.

8. It highlights that individuals with a "High" fee structure tend to have the most credit cards, whereas those with "Low" and "Mid" fee structures show lower counts. This may indicate that higher fee structures are linked to greater credit card usage.

9. It shows a significant gender disparity, with males holding considerably more credit cards than females across all categories.
In conclusion, these plots collectively reveal relationships between various factors and credit card ownership. Individuals from European and American nationalities tend to hold more credit cards, as do those with higher fee structures. Additionally, males dominate credit card ownership, while property ownership appears to correlate with fewer credit cards, suggesting a complex interplay between these factors in financial behavior.

10. The trend indicates a notable disparity in credit card ownership, with Europeans leading significantly. This may be attributed to the fact that Europeans also have the highest number of bank accounts. Having a bank account is often essential for obtaining a credit card, as it establishes a financial relationship with the bank. This correlation suggests that countries with more bank account holders are likely to see increased credit card ownership.

11. 
The High fee structure has the highest count of customers, indicating that a significant number of accounts are associated with higher fees. This may suggest that customers are willing to pay more for premium services or benefits.

The high count in the Private Bank category indicates that many customers prefer private banking services. This could suggest that customers are seeking personalized services or wealth management options. The histogram shows that the Jade loyalty classification has the highest count of customers, indicating it is the most common tier. This suggests that many customers find it accessible and appealing, reflecting effective engagement strategies.


This strong base in the Jade tier presents an opportunity to encourage customers to progress to higher tiers (Gold, Silver, Platinum) by enhancing incentives and rewards, ultimately fostering deeper loyalty and satisfaction.


The Low income band has the highest count, indicating that a significant portion of customers falls into this category. This suggests that the customer base is largely composed of individuals with lower incomes.

12. Majority Behavior: Most individuals or businesses maintain lower balances or accounts, suggesting that financial products are widely used by a large segment of the population, particularly those with modest incomes or savings.

High-Value Accounts: The presence of a long tail on the right side indicates a small number of accounts with significantly higher balances. This highlights the importance of high-net-worth individuals or businesses that may represent valuable customer segments for financial institutions.

Targeted Strategies: Understanding this distribution allows financial institutions to tailor their services effectively. For instance, marketing strategies can focus on enhancing products for the majority while also catering to the specific needs of high-value customers.

Risk Management: The skewness suggests that while most accounts are relatively low-risk, the few high-value accounts may require closer scrutiny to manage potential risks effectively.

Financial Planning: Insights from these distributions can inform financial planning and product development, ensuring that offerings align with the needs of diverse customer segments.

Overall, recognizing the right skewness in these financial variables not only aids in understanding customer behavior but also provides actionable information for better service delivery, risk assessment, and strategic planning in the financial sector.
