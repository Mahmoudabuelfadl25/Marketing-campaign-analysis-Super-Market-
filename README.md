## Marketing-campaign-analysis-Super-Market-(Excel & Tableau)



![image](https://github.com/Mahmoudabuelfadl25/Marketing-campaign-analysis-Super-Market-/assets/150693366/674feafe-74a3-435e-9d74-56a58b77d3cb)



Dashboard online link: https://public.tableau.com/app/profile/mahmoud.abu.elfadl/viz/MarketingAnalysis_17176606462750/Dashboard1?publish=yes




Our recent marketing campaigns have provided us with a wealth of data, offering valuable insights into customer responses and behaviors. This data, segmented by character personas, allows us to tailor our strategies effectively to resonate with different customer profiles. Furthermore, an examination of the distribution of orders by countries gives us a geographical perspective of our market penetration. This information is crucial in identifying potential areas for expansion or improvement. By leveraging these insights, we aim to refine our marketing strategies, enhance customer engagement, and drive growth. This dashboard serves as a comprehensive tool for understanding and visualizing these key metrics and insights.


# Objective


The objective of this data analysis project is to leverage the capabilities of Excel and Tableau to gain meaningful insights from the global supermarket data. The project will begin with data preparation and processing using Excel, where we will clean, organize, and analyze the raw data to ensure its quality and relevance. This stage will involve handling missing values, outliers, and inconsistencies, as well as performing exploratory data analysis to understand the underlying patterns and trends.
Following the data preparation, we will use Tableau to create an interactive dashboard that visually represents our findings. The dashboard will provide a comprehensive view of the supermarket’s performance across various metrics and dimensions, enabling stakeholders to make informed decisions based on data-driven insights.
The ultimate goal of this project is to enhance the supermarket’s operational efficiency, customer satisfaction, and overall profitability by leveraging data analytics.






# Dataset Description


This dataset contains information about customers' interactions with a global supermarket. Each column represents a unique aspect of customer information:


## Columns


- `ID`: Unique identifier for each customer.
- `Year_Birth`: Customer's birth year.
- `Education`: Customer's highest level of education.
- `Marital_Status`: Customer's marital status.
- `Income`: Customer's annual income.
- `Dt_Customer`: Date of customer’s enrollment with the company.
- `Recency`: Days since the customer’s last purchase.
- `MntWines`: Amount spent on wine in the last 2 years.
- `MntFruits`: Amount spent on fruits in the last 2 years.
- `MntMeatProducts`: Amount spent on meat in the last 2 years.
- `MntFishProducts`: Amount spent on fish in the last 2 years.
- `MntSweetProducts`: Amount spent on sweets in the last 2 years.
- `MntGoldProds`: Amount spent on gold products in the last 2 years.
- `NumDealsPurchases`: Number of purchases made with a discount.
- `NumWebPurchases`: Number of purchases made through the company’s web site.
- `NumCatalogPurchases`: Number of purchases made using a catalogue.
- `NumStorePurchases`: Number of purchases made directly in stores.
- `NumWebVisitsMonth`: Number of visits to company’s web site in the last month.
- `AcceptedCmp1 - AcceptedCmp5`: Whether customer accepted the offer in the 1st to 5th campaign.
- `Response`: Whether customer accepted the offer in the last campaign.
- `Complain`: Whether customer raised any complaints.
- `Country`: Country where customer resides.


This dataset is crucial for deriving meaningful insights about customer behavior and the effectiveness of various marketing campaigns.


# Raw Data 
![image](https://github.com/Mahmoudabuelfadl25/Marketing-campaign-analysis-Super-Market-/assets/150693366/dbd96f70-6ab3-4cc5-9458-349744de5f3d)





# Data Processing Steps


The dataset consists of 28 columns and 62,724 rows. The following data processing steps were performed:


## Data Cleaning


1. **Ensure Data Types**: Verify that each column in the dataset is of the correct data type.
2. **Remove Duplicates**: Identify and remove any duplicate entries in the dataset.
3. **Replace Blank Values**: Use the `CTRL + H` shortcut to replace blank values with 0.


## Feature Engineering


1. **Rename Columns**: Rename the columns `NumDealsPurchases`, `NumWebPurchases`, `NumCatalogPurchases`, `NumStorePurchases`, `NumWebVisitsMonth` to `Deals Purchases`, `Web Purchases`, `Catalog Purchases`, `Store Purchases`, `Web Visits Month` respectively.
2. **Add Age Column**: Add a new column named `Age` using the formula `=YEAR(TODAY()) - B2` where `B2` is the cell containing the birth year.
3. **Add Age Category Column**: Establish a new column named `Age Category` to categorize ages into `Youthful`, `Middle-aged` and `Elderly` using the formula `=IF(A2 >= 60, "Old", IF(A2 >= 30, “Middle-aged", "Youhtful"))`.






-  create a new column in our dataset called Income Category. This column will categorize the income levels of our customers into three groups:


 Low  Customers with an income of less than 30,000, 
 Medium Customers with an income between 30,000 and 70,000, 
 High Customers with an income greater than 70,000.


* This categorization will allow us to better understand the income distribution among our customers and tailor our marketing strategies accordingly.

  Data after proccessing
  ![image](https://github.com/Mahmoudabuelfadl25/Marketing-campaign-analysis-Super-Market-/assets/150693366/3ca2af6d-b43d-4684-9640-b6edd6caa778)



# Questions to answer 


- What is the average annual income of our customers?
- Which country has the highest number of customers?
- What is the most common level of education among our customers?
- What is the distribution of marital status among our customers?
- Which product category has the highest sales?
- What is the trend of web visits per month?
- How effective were our marketing campaigns (AcceptedCmp1 - AcceptedCmp5)?
- What is the response rate for our latest marketing campaign?
- How does the spending on different product categories vary with the customer’s income level?




# Conclusion & Recommendations 




- Focus on High-Order Countries: Given that Saudi Arabia has the highest number of orders, it would be beneficial to further investigate the factors contributing to this high demand and apply these strategies in other countries, particularly in the USA where the number of orders is the least.
- Target Married Customers: Since married customers place the most orders, marketing campaigns could be tailored to appeal more to this demographic.
- Engage Graduates More: As graduates account for 51% of orders, consider creating educational or graduate-specific promotions or loyalty programs to maintain and increase engagement with this group.
- Improve Online Presence: Given that store purchases are the most popular, efforts could be made to improve the online shopping experience and promote online deals to increase the number of deal purchases.
- Target Middle-Aged High-Income Customers: As middle-aged customers with high income were the most frequent orderers, consider personalizing marketing campaigns to cater to their preferences and needs.
- Evaluate Marketing Campaigns: The first and last marketing campaigns were the most effective in generating orders. Analyze what made these campaigns successful and apply these strategies to future campaigns.






