# Customer Churn Analysis Project

## Overview
This project analyzes customer churn behavior using various service-related features. The goal is to identify the factors contributing to customer churn and provide actionable insights that can help reduce churn and improve customer retention strategies.

## Introduction
Customer churn is a critical issue for companies, especially in subscription-based businesses. Understanding why customers leave and what factors influence their decision is key to reducing churn rates and maintaining a strong customer base. This analysis examines different service-related factors and their impact on churn to help businesses make data-driven decisions to retain customers.

## Dataset Overview
The dataset consists of customer service information, payment methods, and churn status. Each row in the dataset represents a customer, and the columns represent various aspects of their service usage.

| Column Name         | Description                                                   |
|---------------------|---------------------------------------------------------------|
| **customerID**       | Unique identifier for each customer                           |
| **gender**           | Gender of the customer (Male/Female)                          |
| **SeniorCitizen**    | Whether the customer is a senior citizen (1 = Yes, 0 = No)    |
| **Partner**          | Whether the customer has a partner (Yes/No)                   |
| **Dependents**       | Whether the customer has dependents (Yes/No)                  |
| **tenure**           | Number of months the customer has been with the company       |
| **PhoneService**     | Whether the customer has phone service (Yes/No)               |
| **MultipleLines**    | Whether the customer has multiple lines (Yes/No/No phone service) |
| **InternetService**  | Type of internet service (DSL/Fiber optic/No)                 |
| **OnlineSecurity**   | Whether the customer has online security (Yes/No)             |
| **OnlineBackup**     | Whether the customer has online backup (Yes/No)               |
| **DeviceProtection** | Whether the customer has device protection (Yes/No)           |
| **TechSupport**      | Whether the customer has tech support (Yes/No)                |
| **StreamingTV**      | Whether the customer has streaming TV (Yes/No)                |
| **StreamingMovies**  | Whether the customer has streaming movies (Yes/No)            |
| **Contract**         | Type of contract (Month-to-month/One year/Two year)           |
| **PaperlessBilling** | Whether the customer has paperless billing (Yes/No)           |
| **PaymentMethod**    | Payment method (Electronic check/Mailed check/Bank transfer/Credit card) |
| **MonthlyCharges**   | Monthly charges incurred by the customer                      |
| **TotalCharges**     | Total charges incurred by the customer                        |
| **Churn**            | Whether the customer has churned (Yes/No)                     |

## Key Analysis Steps

1. **Data Loading and Preparation**: Clean and preprocess the dataset.
2. **Exploratory Data Analysis (EDA)**: Visualize service usage and churn rate using count plots.
3. **Churn Analysis**: Analyze customer churn based on services and payment methods.
4. **Visualization**: Generate visual insights into factors affecting customer churn.

## Findings
- **Service Usage**: Customers without value-added services like online security and tech support show higher churn rates.
- **Payment Method Impact**: Electronic check users have a significantly higher churn rate (~45%) compared to other payment methods.
- **Churn and Streaming Services**: Customers with streaming services (TV/movies) tend to have slightly lower churn rates (~25%).

## Recommendations
1. **Promote Value-Added Services**: Encourage adoption of services like online security and tech support to reduce churn.
2. **Improve Payment Method Experience**: Address issues with electronic check payments to lower churn rates.
3. **Service Bundling**: Offer bundled services, such as streaming and tech support, to improve customer satisfaction.

## Technologies Used
- **Python**: Main language for analysis.
- **Pandas**: For data manipulation.
- **Seaborn** and **Matplotlib**: For data visualization.
- **Jupyter Notebook**: For interactive analysis.

## Installation and Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/customer-churn-analysis.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the analysis:
   ```bash
   jupyter notebook TCA.ipynb
   ```

## Project Structure
```
customer-churn-analysis/
│
├── data/                   # Dataset folder
├── TCA.ipynb               # Analysis notebook
├── README.md               # Project documentation
├── requirements.txt        # List of dependencies
└── plots/                  # Generated plots
```

