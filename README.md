# Customer Churn Analysis
## Project Overview
The goal of this project is to analyze customer churn for a telecom company in order to identify important factors and offer practical advice for customer retention techniques.  A thorough dataset that includes information on customer demographics, service subscriptions, account details, and churn status is used in the analysis.  The project aims to lower the turnover rate and decrease related revenue loss by figuring out why customers leave.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Tools & Technologies](#tools--technologies)
4. [Power BI Dashboards](#power-bi-dashboards)
5. [Key Findings & Insights](#key-findings--insights)
    - [Executive Summary](#executive-summary)
    - [Customer Demographics & Profiles](#customer-demographics--profiles)
    - [Contracts & Payment Methods](#contracts--payment-methods)
    - [Product Subscriptions](#product-subscriptions)
    - [Financial & Support Drivers](#financial--support-drivers)
6. [Setup & Usage](#setup--usage)
7. [Project Structure](#project-structure)
8. [Contact](#contact)

## Dataset
- **Total Records**: 7,043 customer entries
- **Total Features**: 23 columns
- **Key Fields**: 
    * `customerID`: Unique customer identifier 
    * **Demographics**: `gender`, `SeniorCitizen`, `Partner`, `Dependents` 
    * **Service Information**: `PhoneService`, `InternetService`, `StreamingTV`, `StreamingMovies`, `MultipleLines`, `OnlineBackup`, `OnlineSecurity` 
    * **Account Details**: `tenure`, `Contract type`, `PaymentMethod`, `MonthlyCharges`, `TotalCharges` 
    * **Support Tickets**: `numAdminTickets`, `numTechTickets` 
    * **Target Variable**: `Churn` (Yes/No)
- Source: [Customer Churn-Dataset](https://github.com/DataVisualizationExpert/Customer-Churn-Analysis-using-Power-BI/tree/main)

## Tools & Technologies
- **Data Cleaning & Preparation**: Python 3.12.5 (with pandas library)
- **Data Visualization & Dashboard Creation**: Power BI

![Python Logo](https://img.icons8.com/color/120/python--v1.png)
![Power BI Logo](https://img.icons8.com/fluency/120/power-bi-2021.png)

## Power BI Dashboards
![Executive Summary](/assets/page1.png)

![Customer Demographics & Profiles](/assets/page2.png)

![Contracts & Payment Methods](/assets/page3.png)

![Product Subscriptions](/assets/page4.png)

![Financial & Support Drivers](/assets/page5.png)

## Key Findings & Insights
The analysis revealed several critical factors influencing customer churn:
### Executive Summary
- **Overall Churn**: 1,869 out of 7,043 customers churned, resulting in a churn rate of 0.27 (27%). 
- **Revenue Impact**: Approximately $139.13K in monthly revenue is lost due to churn. 
- **Average Tenure**: The average customer tenure is 32 months.
### Customer Demographics & Profiles
- **Senior Citizens**: Seniors appear to be churning significantly more (41.68%) compared to non-seniors (23.61%). 
- **Partnership Status**: While customers without a partner have a higher churn rate (32.96% vs. 19.66%), the absolute number of churned customers from the 'with partner' group is still substantial due to their larger proportion in the customer base. 
- **New Customers**: The "0-12 months" tenure group exhibits the highest number of churned customers, suggesting new customers are more likely to churn within their first year.
### Contracts & Payment Methods
- **Contract Type**: Month-to-month contracts have a much higher churn rate and a significantly lower average tenure (18 months) compared to one-year (42 months) and two-year (57 months) contracts. 
- **Paperless Billing**: Customers with paperless billing churn more (19.88%) than those without (6.66%). 
- **Payment Method**: Electronic check and Mailed check appear to have higher churn rates compared to automatic payment methods.
### Product Subscriptions
- **Internet Service**: Fiber Optic internet service has the highest number of churned customers, followed by DSL. Customers with no internet service have the lowest churn. 
- **Multiple Lines**: Customers with multiple lines appear to be more loyal, showing a slightly lower churn rate (12.07%) than those without (14.47%). 
- **Security & Backup Services**: Both Online Security and Online Backup services significantly help retain customers, as subscribers to these services have considerably lower churn rates. 
- **Service Bundles**: As the number of services a customer subscribes to increases, their churn rate generally decreases, indicating that bundled services contribute to higher retention.
### Financial & Support Drivers
- **Monthly Charges**: Higher monthly charges generally correlate with a higher churn rate. 
- **Support Tickets**: Customers who open more support tickets (specifically Admin Tickets) are more likely to churn. 
- **Total Charges**: There is a peak churn in lower total charge bands (e.g., 37% for $0.00 total charges), which then decreases as total charges accumulate, suggesting significant early churn.

## Setup & Usage
To replicate this project locally:
1. **Clone the repository:**
```bash
git clone <repository_url_here>
cd customer-churn-analysis
```
2. **Set up Python environment:**
```bash
python -m venv env
source env/bin/activate  # On Windows: .\env\Scripts\activate
pip install -r requirements.txt
```
3. **Data Cleaning:**
Open and run the `data_cleaning.ipynb` notebook to preprocess the `CustomerChurnDataset.xlsx` and generate `CustomerChurnCleaned.csv`.

## Project Structure
```
CUSTOMER-CHURN-ANALYSIS/
├── assets/                      # Screenshots of Dashboards and logos
├── env/                         # Python virtual environment
├── .gitignore                   # Git ignore file
├── customer_churn_analysis.pbix # Power BI project file
├── CustomerChurnAnalysis.pptx   # Project presentation/report [cite: 1]
├── CustomerChurnCleaned.csv     # Cleaned dataset (generated by data_cleaning.ipynb)
├── CustomerChurnDataset.xlsx    # Original raw dataset 
├── dashboard_structure.txt      # Text file outlining dashboard layout/pages
├── data_cleaning.ipynb          # Jupyter notebook for data cleaning and preprocessing
├── README.md                    # Project README file (this file)
└── requirements.txt             # Python dependencies
```

## Contact
Neehanth Reddy M - [Github](https://github.com/neehanthreddym) [LinkedIn](https://www.linkedin.com/in/neehanthreddy/) [Email](mailto:neehanthreddym@gmail.com)