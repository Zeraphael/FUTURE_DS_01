📊 Online Retail Sales Analysis

📌 Project Overview

In this project, I analyzed sales trends using the Online Retail Dataset obtained from Kaggle:
https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset

The dataset contains transactional data with the following columns:

- InvoiceNo
- StockCode
- Description
- Quantity
- InvoiceDate
- UnitPrice
- CustomerID
- Country

---

🧹 Data Cleaning & Preparation

I used Python (Pandas) to clean and preprocess the dataset.

Key Cleaning Steps:

- Identified 1,454 missing values in the "Description" column
- Identified 135,080 missing values in the "CustomerID" column

👉 These values were not removed or imputed because:

- Missing "CustomerID" may represent anonymous customers
- Removing them would result in significant data loss
- The analysis focused more on sales trends rather than individual customer tracking

---

🔁 Duplicate Values

- Found 5,268 duplicate rows

👉 These were not removed because:

- A customer can make multiple transactions
- A transaction can include multiple products
- These are valid real-world retail scenarios

---

🔄 Data Type Conversion

- Converted "CustomerID" → Integer
- Converted "InvoiceDate" → DateTime

---

💰 Feature Engineering

- Created a new column:
  
  Revenue = Quantity × UnitPrice

---

📊 Dashboard & Analysis (Power BI)

The cleaned dataset was imported into Power BI for visualization.

Key Metrics:

- Total Customers
- Total Transactions
- Total Revenue

---

📈 Analysis Performed:

- Monthly trend of sold quantities
- Yearly revenue comparison (2010 vs 2011)
- Top 10 countries by transaction volume
- Top 10 customers based on purchase volume
- Top 6 most sold products

---

🔍 Key Insights

1. Seasonal Sales Pattern
   
   - Sales peak significantly in December, indicating strong holiday demand.

2. Revenue Growth
   
   - 92.32% of total revenue was generated in 2011, compared to 7.68% in 2010, showing rapid business growth.

3. Geographical Concentration
   
   - The majority of transactions occurred in the United Kingdom, suggesting market dependency.

4. Product Concentration
   
   - A small number of products account for a large portion of total sales.

---

📁 Project Structure

- 📓 Jupyter Notebook (Data Cleaning & Preparation)
- 📊 Power BI Dashboard
- 🖼️ Dashboard Screenshot
- 📄 README

---

🛠️ Tools & Technologies

- Python (Pandas)
- Power BI

---

📌 Conclusion

This project demonstrates the end-to-end data analysis workflow:

- Data cleaning
- Feature engineering
- Exploratory data analysis
- Dashboard creation

The insights generated can help businesses understand sales patterns, customer behavior, and market trends.

---
