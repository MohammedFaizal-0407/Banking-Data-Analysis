# 🏦 Bank Customer EDA — Exploratory Data Analysis

 Python project performing end-to-end **Exploratory Data Analysis** on a banking customer dataset, uncovering behavioral patterns, financial correlations, and customer segmentation insights.

---

## 📂 Files

| File | Description |
|------|-------------|
| `BankEDA_Version_1.ipynb` | Initial EDA — univariate, bivariate, and categorical analysis |
| `BankEDA_Version_2.ipynb` | Enhanced EDA — regression plots, deeper correlation analysis, and written insights |
| `Banking.csv` | Source dataset containing customer banking and demographic data |

---

## 🗃️ Dataset Overview

**Key Columns:**

| Category | Columns |
|----------|---------|
| **Demographics** | Age, Gender, Nationality, Occupation |
| **Financial Accounts** | Bank Deposits, Saving Accounts, Checking Accounts, Foreign Currency Account, Business Lending, Bank Loans, Credit Card Balance, Superannuation Savings |
| **Customer Profile** | Fee Structure, Loyalty Classification, Risk Weighting, Properties Owned, Income Band |
| **Other** | Client ID, Joined Bank date, Branch ID (BRId), Investment Advisor ID (IAId) |

---

## 🔍 Analysis Performed

### ✅ Version 1
- Loaded and inspected dataset (shape, info, describe)
- Created **Income Band** feature — segmenting customers into `Low / Med / High` income brackets
- **Univariate Analysis** — count plots for all categorical columns
- **Bivariate Analysis** — category distributions broken down by Nationality
- **Numerical Analysis** — histogram + KDE plots for 9 financial variables
- **Correlation Heatmap** — identified relationships between financial account balances

### ✅ Version 2 (Enhanced)
- Improved data loading with missing value checks and datetime parsing (`Joined Bank`)
- Expanded numerical columns to include `Age` and `Fee Structure`
- **Regression Plots** on key variable pairs:
  - Bank Deposits vs Saving Accounts
  - Checking Accounts vs Saving Accounts & Foreign Currency Account
  - Age vs Superannuation Savings
  - Estimated Income vs Checking Accounts
  - Bank Loans vs Credit Card Balance
  - Business Lending vs Bank Loans
- Detailed written **insights** for each finding

---

## 💡 Key Insights

**1. Deposits & Savings Behavior**
Customers who maintain high Bank Deposit balances also tend to hold higher Saving and Checking Account balances — suggesting a consistent saving-oriented financial behaviour across account types.

**2. Income, Age & Wealth Accumulation**
Older and higher-income customers show moderate positive correlations with Superannuation Savings, Checking, and Saving Account balances — consistent with typical financial lifecycle trends of progressive wealth accumulation.

**3. Low Correlation with Properties Owned**
Property ownership showed weak correlation with banking variables, likely influenced by external factors such as real estate markets, location, and inheritance — variables not captured in this dataset.

**4. Business vs. Personal Banking**
Business Lending correlates moderately with Bank Loans, suggesting some customers carry both personal and business debt. However, business lending is largely uncorrelated with deposit or property metrics — indicating it serves a distinct customer segment.

---

## 🛠️ Libraries Used

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading, cleaning, feature engineering |
| `numpy` | Numerical operations |
| `matplotlib` | Plotting and chart layout |
| `seaborn` | Statistical visualizations (histplot, countplot, heatmap, regplot) |

---

## 🚀 How to Run

1. Clone the repository and ensure `Banking.csv` is in the same directory
2. Open either notebook in **Jupyter Notebook**, **JupyterLab**, or **Google Colab**
3. Run all cells sequentially (`Runtime → Run All`)

```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook BankEDA_Version_2.ipynb
```

---

## 👤 Author

**Mohammed Faizal** — Data Analyst

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mhd-faizal0407)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/MohammedFaizal-0407)
