# Customer Behaviour Analytics

## Project Overview

This project analyses retail customer shopping behaviour using **Python, SQL, and Power BI**.

The aim is to transform raw customer transaction data into actionable insights that could help a retail business improve **sales performance, customer engagement, and customer loyalty**.

The project follows an end-to-end data analytics workflow:
1. Business Problem & Raw CSV data
2. Data cleaning, modelling and EDA in Python
3. Data analysis in SQL
4. Interactive Power BI dashboard
5. Project report
6. Presentation

**Problem:** A retail company wants to better understand its customers' shopping behaviour in order to improve sales, customer satisfaction, and customer loyalty. The management team has observed changes in purchasing patterns and want to know which factors drive consumer decisions and repeat purchases.

**Objective:** Leverage customer shopping data to identify meaningful trends and patterns that could support business decision-making.

---

## Dataset

The project begins with a raw CSV file containing customer shopping data such as:

* **Customer demographic information**
* **Items purchased**
* **Purchase amounts**
* **Review ratings**
* **Are they apart of a subscription service?**
* **Has a discount been applied?**
* **Payment methods**


An important part of this project is recognising that real-world business data is rarely perfect or complete.

For this project, I intentionally worked with a **limited set of variables** to simulate a realistic business scenario where an organisation or client may not collect or provide specific data due to **privacy, security, or data governance requirements**.

This means that some potentially useful variables (e.g. browsing behaviour) are not available for analysis and, therefore, i have treated it as part of the **analytical challenge**.

---

## EDA in Python

I cleaned and transformed the dataset to improve data quality, consistency, and usability for further analysis.

* Replaced the 37 missing `Review Rating` values with the **median rating of the corresponding product category**, rather than using the overall dataset median. This helps preserve differences in rating patterns between product categories.
* Renamed the dataset columns using snake_case to improve readability and maintain consistent naming conventions throughout the analysis.
* Split `age` values into distinct age groups to make demographic patterns easier to analyse.
* Converted the `Frequency of Purchases` categorical values into numerical values to make them easier to analyse quantitatively.
* Removed the `Promo Code Used` column because it contained the same information as `Discount Applied`, making it redundant for the analysis.

