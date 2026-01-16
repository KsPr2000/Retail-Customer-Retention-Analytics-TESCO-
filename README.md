Retail Customer Retention Analytics – TESCO 
 
Project Overview: 
 
TESCO, a retail leader in the UK, operates across multiple cities through superstores, express 
outlets, and online channels. With growing competition and changing customer expectations, 
customer retention has become increasingly difficult. Although TESCO has access to rich data 
on customer transactions, store performance, and loyalty programs, their current reporting 
system lacks the analytical depth needed to: 
 
● Understand why customers are churning? 
(Customer churn, the rate at which customers stop doing business with a company) 
 
● Identify high-value customers and those at risk. 
 
● Evaluate the impact of loyalty tiers and promotions. 
 
● Guide store-specific retention strategies 
 

 
Project Objective: Develop a robust, Interactive Customer Retention Analytics Dashboard in 
Power BI using the provided data, which will: 
 
● Consolidate customer demographics, transaction history, store performance, and 
loyalty program usage. 
● Enable dynamic segmentation of high-value, repeat, and churned customers. 
● Offer actionable insights for improving retention, loyalty program effectiveness, and 
regional store strategies. 
 

 
Dataset Description:  
 
1. Customer_Demographics.csv: Contains demographic and membership details for each 
TESCO customer. Used to segment customers based on age, gender, region, income 
level, and membership tenure. 
                                                                                                                      
 
 
2. Customer_Transactions.csv: Logs individual purchase transactions by customers across 
TESCO stores. Used for purchase behavior, frequency, and loyalty analysis. 
 
 
 
3.Store_Locations.csv :  Contains metadata about TESCO store locations. Supports store-wise 
performance and retention analysis. 
 
 
 
4. Loyalty_Program.csv :Tracks customer participation in TESCO’s loyalty program. Used for 
analyzing points behavior, tier effectiveness, and redemption trends. 
 
                                                                                                                      
 
 
5. Churn_Labelled_Customers.csv : Provides a churn flag and behavioral insight for each 
customer based on the date of last purchase. Supports churn rate analysis and customer 
reactivation strategies. 
 
 
 
               
Task to be performed:  

Task 1: Data Modeling and Cleaning  
 
Goal: Prepare the data for analysis 
 
● Use Power Query Editor to load and transform the datasets. 
○ Remove duplicate rows based on key columns (e.g., Customer_ID, Store_ID) 
○ Format columns: Convert dates, ensure numeric types for Amount, Points, etc. 
○ Handle missing or null values appropriately (e.g., filter or replace) 
● Create calculated columns: 
○ Membership_Duration = Today - Membership_Since 
○ Add a Transaction_Year and Transaction_Month column from Transaction_Date 
● Create a basic Data Model view  
○ One-to-Many: Customer_Demographics → Transactions, Loyalty_Program, 
Churn_Labelled_Customers 
○ Many-to-One: Transactions → Store_Locations 
 
Task 2: Churn and Retention Metrics 
 
 
Goal: Identify churn trends across segments 
 
                                                                                                                      
● Create a Churn Rate card: (Churned Customers / Total Customers) * 100 
● Visualize churn rate by: 
○ Region 
○ Income Group 
○ Store Type (via store join) 
○ Identify top 5 segments with highest churn % 
● Create funnel chart: Total Customers → Repeat → Churned 
 
Task 3: Repeat Purchase Analysis  
 
Goal: Understand customer loyalty through repeat behavior 
● Create a measure: 
Low-Tier Customers: (2-4 purchases) 
Mid-Tier Customers: (5-10 purchases) 
High-Tier Customers: (11+ purchases) 
● Compare avg. purchase frequency by: 
○ Region 
○ Age Group 
○ Loyalty Tier 
 
● Identify product categories most frequently bought by loyal customers 
 
Task 4: Promotion & Loyalty Impact  
 
Goal: Evaluate how promotions and loyalty tier affect retention 
● Create Measure: 
○ % of transactions where promotion was applied 
○ Avg. purchase amount with vs without promotion 
 
● Compare churn rate across loyalty tiers 
● Show Points Earned vs Redeemed by Tier using clustered column chart 
● Recommend how to improve redemption and retention 
 
Task 5: Store Performance vs Retention  
 
Goal: Link store characteristics to retention outcomes 
● Merge Store_ID from transactions with Store_Locations 
● Visualize: 
○ Avg. transaction amount by store type 
○ Churn rate by store region 
○ Correlation between store opening year and retention 
● Suggest where to run store-specific campaigns 
 
 
                                                                                                                      
Task 6: Customer Value (CLV) Analysis 
 
Goal: Identify and prioritize high-value customers 
Calculate CLV = Total Amount Spent / Membership Duration (in years) 
  
● Segment customers into: 
 
○ Low (Bottom 25%) 
○ Medium (Mid 50%) 
○ High (Top 25%) 
 
● Visualize: 
○ CLV vs Days Since Last Purchase 
○ CLV by Loyalty Tier and Region 
 
Task 7: Final Dashboard  and Executive summary 
 
Goal: Communicate insights for business action 
● Create a multi-page Power BI report: 
 
○ Page 1: Overview KPIs (Churn, CLV, Repeat Rate) 
○ Page 2: Loyalty & Promotion Impact 
○ Page 3: Store and Region Insights 
○ Page 4: Customer Segmentation (Churned, Repeat, High-Value) 
 
Add slicers: Region, Income Group, Loyalty Tier, Store Type 
● Create a card or textbox summarizing top 3 recommendations: 
● What should TESCO do to retain more customers? 
● Where should they focus next? 
 

 

 
 
 
 
                                                                                                                      
 
 
 

 
 
                                                                                                                      
 

 
 
 
 
 
 
                                                                                                                      
