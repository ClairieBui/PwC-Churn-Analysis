# **Churn Dashboard Analysis - Power BI Dashboard**
## 📌 **Project Overview**
This project delivers an extensive data visualization platform focused on customer churn metrics. Built for both operational insights and strategic planning, the Power BI dashboards highlight trends, key metrics, and essential performance indicators (KPIs) vital to business operations.
## ❓ **Problem Statement**
PwC is struggling to understand its churn metrics. The key areas of concern include:
- **Churn rate**: The percentage of customers who discontinue their service over a given period. In the dataset, "Churn" is a categorical column (Yes/No), indicating whether a customer has left. 
- **Number of customers at risk**: The count of customers who are likely to churn based on historical data and key indicators like tenure, contract type, and billing method. This can be inferred by filtering customers with "Churn = Yes." 
- **Number of TechTickets**: The number of technical support requests a customer has made, recorded in the "numTechTickets" column. 
- **Number of AdminTickets**: The number of administrative-related support requests a customer has made, recorded in the "numAdminTickets" column. 
- **Total charges**: The total amount a customer has been billed for services, recorded in the "TotalCharges" column.

## 🛠️ **Skills Demonstrated**
- __Power BI__ for data visualization, modeling, and analysis.

## 📊 **Dataset Information**
- **Source**: Excel file containing sales data.
- **Key Columns**:
  - `Customer`
  - `Gender`
  - `SeniorCitizen`
  - `Tenure`
  - `PhoneService`
  - `MultipleLines`
  - `InternetService`
  - `OnlineSecurity`
  - `OnlineBackup`
  - `DeviceProtection`
  - `TechSupport`
  - `StreamingTV`
  - `Contract`
  - `PaperlessBilling`
  - `PaymentMethod`
  - `TotalCharges`
  - `numAdminTickets`
  - `numTechTickets`
  - `Churn`
  ## 🔄 **Data Transformation**
The dataset was processed using Power Query to enhance data structure and analytical capabilities. Instead of following a strict star schema, the data model consists of a primary fact table (Churn) and multiple calculated measure tables for deeper analysis.
Main Data Table:
- Churn Table: The core dataset containing customer-level information, including Churn, Contract, Customer Subscription, customerID, Dependents, DeviceProtection, gender, MonthlyCharges, InternetService.
Calculated Measure Tables:
- Key Measures: Holds calculated values such as % females, % males, Churn rate, and Current Customers to provide quick insights.
- Account Table: Summarizes account-related percentages, including % Contract, % Paperless Billing, and % Payment Method.
- Service Table: Contains aggregated metrics for service features such as % Device Protection, % Multiple Services, % Online Backup, and % Online Security.
- Demographic Key Measures: Provides demographic breakdowns, including % Dependants, % Partner, and % Senior Citizen.

## 📐 **Data Modeling**
This structure relies on a single fact table (Churn) combined with calculated measure tables. This approach enhances data analysis by precomputing key insights, making it easier to track customer churn patterns and service engagement.
![image](https://github.com/user-attachments/assets/fae9614f-c79e-450d-a6ac-0dcf69bd1b6e)

## 📈 **Analysis & Visualizations**
1. Overview dashboard
![image](https://github.com/user-attachments/assets/a4539cb0-3e6a-4827-8404-0d78aae084a1)
- Churn Rate & Customers at Risk: The overall churn rate is 26.54%, with 1,869 customers at risk of leaving. High churn indicates potential service or pricing issues that need addressing.
- Contract Type & Churn Risk: 55.02% of customers are on month-to-month contracts, which are more prone to churn. Customers with one-year and two-year contracts show lower churn rates, suggesting that longer-term contracts improve retention.
- Payment Methods & Churn Risk: Electronic check users (33.58%) have the highest churn risk, potentially due to payment inconvenience or financial instability.
Customers using automated bank transfers or credit card payments have lower churn, indicating that automatic payments contribute to customer retention.
Internet Service Type & Churn
- Fiber-optic users (43.96%) have the highest share of internet service users. The churn risk for fiber-optic customers may be linked to service quality or pricing issues, requiring further investigation.
- Tenure & Churn Risk: 31.04% of customers are in their first year, the highest percentage among tenure groups. Churn rates are typically highest among first-year customers, emphasizing the need for better onboarding and early retention strategies.
- Paperless Billing: 59% of customers use paperless billing, but 41% still opt for paper bills.
Encouraging more customers to switch to paperless billing may improve engagement and reduce churn.
2. Analysis dashboard
![image](https://github.com/user-attachments/assets/b9ab18a4-4f06-4d8b-ba6a-20b3d93c9dcb)

- High Churn Risk for Month-to-Month Contracts: Customers on month-to-month contracts have the highest churn rate (42.71%), significantly higher than two-year (2.83%) and one-year (11.27%) contracts. This suggests that customers with short-term commitments are more likely to leave, likely due to pricing flexibility or dissatisfaction.
Internet Service Impact on Churn
- Fiber-optic users have the highest churn rate (41.89%), while DSL and other services show lower churn (18.6% and 7.4%, respectively). This may indicate issues with service quality, pricing, or competition in fiber-optic offerings.
- Payment Method Correlation with Churn: Electronic check payments are associated with the highest churn rate, indicating that customers using this method may have a weaker commitment or financial instability.
- Automated payments (credit card/bank transfer) correlate with lower churn, suggesting businesses should promote auto-payment options to improve retention.
- Customer Tenure and Churn: First-year customers have the highest churn rate (47.41%), emphasizing the need for stronger onboarding and engagement strategies early in the customer lifecycle. Churn decreases significantly after two years, indicating that long-term customers are more loyal.
- Admin Tickets and Churn: Customers with more administrative support tickets have a higher churn risk, suggesting dissatisfaction with service. Improving customer support could help reduce churn.

## 📌 **Conclusion & Recommendations**
**Conclusions**
- Customers with month-to-month contracts and those paying via electronic checks are more likely to churn.
- Fiber-optic service users show higher churn rates, possibly due to service quality concerns or pricing issues.
- Customers in their first year have the highest churn, emphasizing the need for strong onboarding and early retention efforts.
- Engagement with Multiple Services: 45.48% of customers subscribe to multiple services, reflecting strong interest in bundled offerings.
- Balanced Gender Distribution: Adoption of services is nearly evenly split between genders, indicating no significant preference based on gender.
- Contract Preferences & Churn Risk: Month-to-month contracts make up 88.5% of subscriptions, highlighting customer preference for flexibility but also posing a higher churn risk.
- Payment Methods & Churn Correlation: Electronic checks are the most frequently used payment method but are also associated with higher churn rates.

**Recommendations**
- Targeted Retention for Month-to-Month Customers: Offer discounts or loyalty programs to encourage longer contract commitments.
- Improve Onboarding for First-Year Customers: Provide personalized support and engagement strategies to reduce early churn.
- Address Fiber-Optic Service Issues: Investigate and resolve potential service quality or pricing concerns.
- Promote Paperless Billing: Increase awareness of benefits (e.g., convenience, eco-friendliness) to improve customer engagement.
- Encourage Automatic Payment Methods: Provide incentives for customers to switch from electronic checks to automated bank transfers or credit cards.
- Address service quality or pricing concerns for fiber-optic users.
- Strengthen early-stage customer retention efforts, particularly in the first year.
- Enhance customer support to improve overall satisfaction and reduce churn.

## 🚀 **How to Use This Dashboard**
1. **Download the `.pbix` file** from the repository.
2. **Open Power BI Desktop** and load the file.
3. Use filters and slicers to explore insights interactively.

---
🔗 *For further improvements, feel free to fork this project and contribute!* 🚀




