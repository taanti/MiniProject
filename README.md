# CRISP-DM Supermarket

This repository contains the code and data for the CRISP-DM Supermarket project. The project is part of the Data Analytics mini project for understanding the CRISP-DM process. The project is based on the CRISP-DM process and the data is from a supermarket. For the project, we will be using the CRISP-DM process to analyze the data and provide insights.

The CRISP-DM process is a data mining process framework that describes common approaches used by data mining experts. It is the most widely-used analytics model. The CRISP-DM process includes the following steps:

## 1. Business Understanding

- Background : The dataset represents sales transactions from a supermarket spanning from January 1st, 2019 to March 30th, 2019. It contains information about customer demographics, products sold, pricing, and payment details. Understanding this data can provide valuable insights into sales performance, customer behavior, and product popularity. By analyzing this dataset, businesses can optimize their strategies, enhance customer experiences, and drive revenue growth.

- Main Questions :
  1.  Which cities are the top performers in terms of sales?
  2.  What are the most common payment methods used by customers?
  3.  What types of products do people buy the most by gender?
  4.  Which product lines are the best-selling?
  5.  Which types of customers generate the most revenue?

## 2. Data Understanding

- Data contain transactional data from a supermarket in January 2019 to March 2019.
- Source: [Kaggle](https://www.kaggle.com/aungpyaeap/supermarket-sales)
- The dataset has 10 column and 1000 rows
- Data Dictionary:
  - Invoice ID: Unique identifier for the transaction
  - Branch: Branch of the supermarket
  - City: City where the supermarket is located
  - Customer type: Type of customer (Member or Normal)
  - Gender: Gender of the customer.
  - Product Line: Category of the product purchased.
  - Unit Price: Price per unit of the product.
  - Quantity: Number of units purchased.
  - Tax: 5% tax fee for customer buying.
  - Total: Total price including tax.
  - Date: Date of purchase.
  - Time: Purchase time (10am to 9pm).
  - Payment: Payment used by customer for purchase.
  - COGS: Cost of goods sold.
  - Gross Margin Percentage: Gross margin percentage.
  - Gross Income: Gross income.
  - Rating: Customer stratification rating on their overall shopping experience (On a scale of 1 to 10).

## 3. Data Preparation

- Code Used:
  - Python Version: 3.7.6
- Packages:
  - Pandas, Numpy, Matplotlib, and Seaborn

## 4. Data Cleaning

- Check for missing values :
  By checking the information from the data in the dataset used, it is known that there are no missing values , so no data imputation is performed on the dataset used.
- Check for data types :
  The data type of the 'Date' column was converted from object to datetime64 to facilitate time-based analysis. Additionally, the DataFrame index was set to the 'Date' column to streamline time-based operations.

## 5. Exploratory Data Analysis

- Which cities are the top performers in terms of sales?

    <div align="center"><img src="https://github.com/sisatput/LearnPythonImg/blob/main/CRISP-DM%20Supermarket/Top%20Performers.png"/></div>

From the image, it can be seen that Naypyitaw emerged as the leader in sales when analyzing key metrics such as total revenue, average sales per transaction, and sales growth rate. Its consistently strong performance in these areas confirms its position as the city with the highest sales, providing important insights into its economic prowess and dominance in the market.

- What are the most common payment methods used by customers?

    <div align="center"><img src="https://github.com/sisatput/LearnPythonImg/blob/main/CRISP-DM%20Supermarket/Common%20Payment.png"/></div>

From the chart above, it can be seen that E-wallets are growing in popularity compared to cash, indicating that more and more people prefer digital transactions. However, cash is still widely used, indicating that many people still prefer traditional methods. Credit card usage is not very high, suggesting that there is still room to encourage its use or make it more attractive. This suggests that businesses can capitalize on the popularity of e-wallets, accommodate those who still prefer cash, and make credit cards more attractive to cater to different customer preferences.

- What types of products do people buy the most by gender?

    <div align="center"><img src="https://github.com/sisatput/LearnPythonImg/blob/main/CRISP-DM%20Supermarket/Buy%20Product%20by%20Gender.png"/></div>

Based on the data analysis, it is clear that there are clear differences in the types of products preferred by different genders. Men tend to gravitate towards purchases in the “Food and Beverage” category, whereas women show a stronger inclination towards products categorized under “Health and Beauty”. These gendered buying patterns indicate different preferences and priorities among consumers, highlighting the importance of gender-specific marketing strategies and product offerings in meeting the needs and interests of diverse consumers.

- Which product lines are the best-selling?

    <div align="center"><img src="https://github.com/sisatput/LearnPythonImg/blob/main/CRISP-DM%20Supermarket/Best%20Selling%20Product%20Type.png"/></div>

Based on the chart, Fashion accessories emerge as the best-selling product line, with 178 transactions, closely followed by Food and beverages with 174 transactions. Electronic accessories secured the third position with 170 transactions. This data emphasizes the strong demand for fashion accessories and food and beverages, highlighting the importance of catering to customer preferences across various product categories.

- Which types of customers generate the most revenue?

    <div align="center"><img src="https://github.com/sisatput/LearnPythonImg/blob/main/CRISP-DM%20Supermarket/Customer%20Type.png"/></div>

From the data presented, an analysis of customer types in the sales records unveils two distinct categories: regular customers and members. Among these, members stand out as the primary revenue generators, boasting a substantially higher total spend compared to regular customers. This observation underscores the pivotal role of customer loyalty programs and highlights the potential advantages of offering membership incentives to bolster both revenue generation and customer retention efforts.

## 6. Summary

- Naypyitaw leads in sales, indicating market dominance.
- E-wallets are growing, cash remains popular, and credit card use is low.
- Gender-specific preferences: men favor "Food and Beverage," women prefer "Health and Beauty."
- Fashion accessories and food/beverages are top sellers.
- Revenue is primarily driven by members, underscoring the importance of loyalty programs.
