# Credit-Card-Fraud-Risk-Analysis

## Project Overview
This project focuses on analysing credit card transactions to identify fraudulent activities, assess financial exposure and evaluate potential weaknesses in fraud detection. An interactive power BI dashboard was developed to examine transaction patterns, fraud rates, transaction values, merchant categories, customer demographics and transaction timing. The objective is to provide actionable insights that can help financial institutions strengthen fraud prevention controls, identify high-risk transaction patterns and improve financial risk management. 

<img width="793" height="457" alt="WhatsApp Image 2026-11-08 at 00 10 34" src="https://github.com/user-attachments/assets/d23789e5-87f8-47de-984a-7d226586179d" />


## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results and Findings](#results-and-findings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)
---
### Data Sources

2 CSV files obtained from Kaggle were used for this project:

* Credit Card Fraud Training Dataset 
* Credit Card Fraud Testing Dataset
  
  [Download Kaggle Dataset Here](https://www.kaggle.com/datasets/kartik2112/fraud-detection)
  
The datasets contain credit card transaction records with the following information:

* Transaction date and time.
* Credit card number.
* Merchant.
* Transaction category.
* Transaction amount.
* Customer gender.
* Customer location.
* Merchant location.
* Transaction identification number.
* Fraud classification (is_fraud).

The training dataset contains 1,048,575 records, while the testing dataset contains 555,719 records.

The two datasets were combined to create a consolidated transaction table containing 1,604,294 records for analysis.

---
### Tools

The following tools and technologies were used:

* Excel CSV: Source data storage and import.
* DAX: Creation of calculated columns, financial measures and fraud performance indicators.
* Power Query: Data extraction, transformation and cleaning.
* Microsoft Power BI Desktop: Dashboard development, data modelling, visualisation and reporting.
* GitHub: Project documentation and portfolio presentation.
---
### Data Cleaning and Preparation

Data preparation was carried out using Power Query in Power BI. The following are the majorcleaning activities carried out:

- Imported the training and testing datasets into Power BI.
- Examined both datasets to understand their structures and column names.
- Checked that the datasets had compatible columns before appending.
- Appended the training and testing datasets into one consolidated table named Fraud_Transactions.
- Reviewed data types and converted transaction dates, numerical fields and categorical fields into appropriate formats.
- Checked for missing values and duplicate transaction records.
- Retained transaction identifiers as text to preserve their original values.
- Created additional date and time fields to support time-based analysis.
- Derived transaction year, month, month number, day, day number and transaction hour.
- Created transaction time-period classifications to support analysis across morning, afternoon, evening and night.
- Created additional classifications to support transaction amount and customer demographic analysis.
- Validated the fraud classification field to distinguish fraudulent transactions from legitimate transactions.
---
### Exploratory Data Analysis 

Exploratory Data Analysis was conducted to understand transaction characteristics and identify patterns associated with fraudulent activities. This provides a foundation for selecting relevant fraud indicators and designing the Power BI dashboard. The following are the areas of focus:

* Distribution of fraudulent and legitimate transactions.
* Transaction volume and transaction value.
* Fraud cases across merchant categories.
* Fraud distribution across different time periods.
* Fraud rates by customer gender.
* Transaction amounts by fraud status.
* Fraud patterns across transaction dates and hours.
* Geographic distribution of transactions.
* Identification of transaction categories with relatively high fraud activity.
---
### Data Analysis

DAX measures and calculated columns were developed to support the analysis.

The main performance indicators are:

* Total Transactions.
* Total Transaction Amount.
* Total Fraud Cases.
* Average Transaction Amount.
* Fraud Rate (%).
* Fraudulent Transaction Amount.
* Average Fraudulent Transaction Amount.
* Fraud Amount Exposure (%).

The dashboard was designed around the following analytical areas:

1. Fraud Cases by Transaction Category: This examines the distribution of fraudulent transactions across merchant categories to identify categories with higher fraud activity.

2. Fraud Cases by Time Period: Evaluates fraudulent activities across morning, afternoon, evening and night periods to identify potential time-related patterns.

3. Average Transaction Amount by Fraud Status: It compares the average transaction values of fraudulent and legitimate transactions.

4. Fraud Rate by Gender: This examines differences in observed fraud rates across customer gender groups.

5. Fraud Rate by Transaction Date and Time: Analyses how fraud rates vary across transaction days and times to identify periods of increased fraud activity.

6. Fraud Cases by Merchant Category: This ranks merchant categories according to the number of fraudulent transactions recorded.

Interactive slicers were incorporated to allow users to filter the dashboard by relevant merchant, transaction amount and geographic attributes.

---
### Results and Findings

The results and findings from the analysis are summarised as follows:

- A total of 658 fraudulent cases were identified within the displayed transaction population, highlighting the need for continuous fraud monitoring.
- The fraud rate stood at 0.64%, showing that fraudulent transactions represented a measurable proportion of the transactions under analysis.
- The average transaction amount was $71.49, providing a benchmark for assessing transaction values and identifying potentially unusual activity.
- The fraud cases by transaction category chart revealed differences in fraud concentration across merchant categories, highlighting the importance of category-specific fraud monitoring.
- The time-period analysis showed that fraudulent transactions were not evenly distributed across the day. This suggests that transaction timing is a useful dimension for further fraud-risk investigation.
- The average transaction amount comparison showed a substantial difference between fraudulent and legitimate transaction values, suggesting that transaction amount can contribute to risk-based monitoring.
- The gender analysis revealed differences in observed fraud rates between male and female customers, providing an additional dimension for understanding transaction patterns.
- The merchant category analysis identified varying concentrations of fraudulent transactions across merchants, supporting the need for targeted monitoring and risk assessment.
---
### Recommendations

Based on the analysis, the following recommendations are proposed:

- Strengthen transaction monitoring to identify unusual transaction patterns and suspicious activities.
- Prioritise high-risk merchant categories for additional fraud prevention controls 
- Periods with higher fraud activity should be considered for additional verification measures where appropriate.
- Risk-based transaction screening should be applied to identify potentially suspicious transactions.
- All fraud detection controls should be strengthened.
- Unusual transaction locations and geographic inconsistencies should be investigated as part of broader fraud-risk assessments.
- Regular fraud reporting should be provided with management.
- Continuous evaluation of fraud models should be carried out to identify weaknesses and improve detection accuracy.
---
### Limitations

The following limitations were observed in the course of the project:

* The analysis is based on historical transaction records and may not reflect current fraud patterns.
* The dashboard figures depend on the selected filters and should be interpreted within their applicable filter context.
* Fraud patterns identified in the dataset may not represent all forms of credit card fraud.
* Differences in fraud rates across gender, merchant category or transaction time do not establish causation.
* The analysis identifies patterns and associations but does not independently establish the reasons behind fraudulent activities.
* The dataset does not provide complete information about whether fraudulent transactions were successfully blocked, recovered or resulted in actual financial losses.
* The dashboard is an analytical and monitoring tool, not a real-time fraud prevention system.
* Further model validation would be required before using the identified patterns for automated fraud classification.
---
### References
- Credit card fraud Dataset from [Kaggle](https://www.kaggle.com/datasets/kartik2112/fraud-detection)
- Various learning resourses on Youtube
---
