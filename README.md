# Customer Churn Prediction & Retention Strategy

This project analyzes customer churn behavior using the **Telco Customer Churn dataset**. The objective is to identify which customers are likely to churn and propose actionable strategies to improve customer retention — **without relying on machine learning**.

---

## Objective

- Understand key factors driving customer churn.
- Segment customers based on churn risk.
- Propose **data-driven retention strategies**.

---

## Dataset

- **Source**: [Telco Customer Churn on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Size**: ~7,000 customer records
- **Features**: Demographics, account info, service usage, contract type, etc.

---

## Tools & Technologies

- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Jupyter Notebook

---

## Data Cleaning

- Converted `TotalCharges` to numeric
- Replaced empty strings with `NaN` and filled or dropped as needed
- Encoded categorical features (e.g., Yes/No, Contract types)
- Removed duplicates and ensured data integrity

---

## Exploratory Data Analysis (EDA)

Key Insights:
- Customers on **month-to-month contracts** are more likely to churn.
- **Fiber optic** users churn more than DSL users.
- **Senior Citizens** have a higher churn rate.
- Customers with **paperless billing** or **higher monthly charges** tend to churn.

Visuals include:
- Churn distribution
- Tenure vs Monthly Charges heatmaps
- Contract type vs Churn bar plots

---

## Churn Risk Segmentation

Customers were segmented as "**At Risk**" if they:
- Have month-to-month contracts
- Low tenure (e.g., < 12 months)
- High monthly charges (e.g., > $70)
- Use paperless billing

This segmentation allows targeted retention actions without using ML.

### Example Visualization:
![At-Risk vs Others Churn Rate](assets/churn_risk_segment.png)

---

## Retention Strategy Recommendations

1. **Lock-in Contracts**: Encourage longer contracts (1–2 year) via promotions or discounts.
2. **Loyalty Benefits**: Reward long-tenure customers to improve satisfaction and reduce churn.
3. **Support First**: Target at-risk customers with proactive customer support and outreach.
4. **Bundled Offers**: Reduce cost sensitivity by offering value-based bundling.

---

## Project Structure

```bash
📦Telco-Churn-Analysis/
├── data/
│   └── Telco-Customer-Churn.csv
├── notebooks/
│   └── Telco_Customer_Churn_Analysis.ipynb
├── assets/
│   └── churn_risk_segment.png
├── README.md
└── requirements.txt
