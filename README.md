# Hi, I'm Enoch Kanikwu

First Class Statistics graduate (Bowen University, 4.81/5.0) working in data analysis and data engineering. I build tested pipelines on real Nigerian data, and I check the data before I trust it.

## Projects

### [Naira Rates Monitor](https://github.com/ebukachukwu-hub/naira-rates-monitor)
A scheduled Databricks job that collects the Central Bank of Nigeria's official exchange rates every day (62,000+ records, 13 currencies since 2001) and checks them for errors.

- Found values up to 10,000 times the true rate, swapped currencies and conflicting duplicates in the official history
- Tested the obvious duplicate rule ("keep the later entry") and found it wrong in 17 of 21 serious cases, then replaced it
- Separates typos from real naira moves by removing each day's market-wide move first: 210 problem values found out of 62,205
- PySpark, Databricks (Delta, Unity Catalog, Jobs), 31 tests in GitHub Actions

### [Nigeria Food Price Intelligence Pipeline](https://github.com/ebukachukwu-hub/nigeria-food-price-intelligence)
A Bronze, Silver and Gold pipeline on the World Bank's food price data for 73 Nigerian markets, measuring which foods have the most volatile prices.

- Traced a December 2025 error (milk in 21 Borno markets at about 5% of its normal price) to the World Food Programme's own data
- Showed that one such entry made a single market look like the most volatile series in the dataset (volatility 0.84, falling to 0.09 without it)
- Found milk, fish and onions the most volatile foods in the northeast under six different settings
- PySpark, Databricks, 19 tests in GitHub Actions

### [Crop Recommendation Web App](https://github.com/ebukachukwu-hub/crop-recommendation-app)
A machine learning model that recommends crops from soil and environmental conditions, deployed as a Flask web application.

### [Retail Sales ETL Pipeline](https://github.com/ebukachukwu-hub/Retail_ETL_Project)
A modular PySpark ETL pipeline that validates retail transactions against business rules for revenue reporting.

## Writing

[Check the Data Before You Trust It: Two Pipelines on Nigerian Public Data](#) (LinkedIn article)

## Skills

Python · SQL · PySpark · Databricks · Delta Lake · Excel · R · Statistics · pytest · GitHub Actions

## Contact

[LinkedIn](https://www.linkedin.com/in/enoch-kanikwu-470053305) · enochkanikwu@gmail.com
