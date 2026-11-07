# Email Campaign Analysis | Hypothesis Testing Using Python

## 📌 Project Overview

This project analyzes an e-commerce marketing campaign dataset to investigate whether customers exposed to an Email campaign spend differently per order compared with customers in the Control group.

The analysis uses Python, Exploratory Data Analysis (EDA), data visualization, and statistical hypothesis testing to identify differences in customer spending behaviour and derive actionable business insights.

## 🎯 Business Problem

Does the Email campaign result in a statistically significant difference in average order value compared with the Control group?

The objective is to evaluate customer spending behaviour and understand whether the Email campaign shows a measurable difference compared with the Control group.

## 📂 Dataset Overview

- Total customers: 1,200
- Campaign groups: Control, Email, Social Media
- Key variables:
  - Customer_ID
  - Campaign_Group
  - Age
  - Gender
  - Website_Visits
  - Session_Minutes
  - Purchase_Made
  - Order_Value_INR
  - Satisfaction_Before
  - Satisfaction_After

## 🛠️ Tools & Technologies

- Python
- Pandas – Data manipulation and cleaning
- NumPy – Numerical operations
- Matplotlib – Data visualization
- SciPy – Statistical hypothesis testing
- Jupyter Notebook

## 🔍 Analysis Workflow

### 1. Data Cleaning
- Checked missing values.
- Checked duplicate records.
- Verified Customer_ID uniqueness.
- Converted numerical columns to appropriate data types.
- Investigated outliers using boxplots.

### 2. Exploratory Data Analysis (EDA)
- Analyzed overall purchase distribution.
- Compared the number of buyers across campaign groups.
- Visualized order value distributions.
- Compared spending patterns between Email and Control groups.

### 3. Hypothesis Testing

**Test:** Welch's Independent Two-Sample T-Test

**Null Hypothesis (H0):** There is no significant difference in mean order value between Email and Control buyers.

**Alternative Hypothesis (H1):** There is a significant difference in mean order value between Email and Control buyers.

**Significance Level:** 0.05

### 4. Results

| Metric | Control | Email |
|---|---:|---:|
| Number of buyers | 92 | 113 |
| Mean order value | ₹633.60 | ₹716.23 |
| Standard deviation | ₹191.43 | ₹176.09 |

**Statistical Test Results:**

- T-statistic: 3.19
- P-value: 0.0017
- Difference in means: ₹82.63
- Relative difference: Approximately 13% higher for Email.

**Decision:** Reject the null hypothesis because the p-value is below 0.05.

## 💡 Key Business Insights

1. Email had 113 buyers compared with 92 in the Control group.
2. Average order value among Email buyers was approximately 13% higher.
3. The difference in average order value was statistically significant.
4. Email appears promising as a campaign channel, but purchase conversion rates and campaign costs should also be evaluated.

## 📊 Business Recommendation

Further evaluate the Email campaign by analyzing purchase conversion rates and campaign costs before making a final decision about its overall effectiveness.

## ⚠️ Limitations

- The spending comparison considers only customers who made a purchase.
- Statistical significance does not establish causation.
- Campaign costs and return on investment were not included.
- Outlier removal may influence the results and should be evaluated through sensitivity analysis.

## 📁 Project Files

- `notebooks/` – Python analysis and hypothesis testing.
- `data/` – Dataset used for analysis, if redistribution is permitted.
- `visuals/` – Charts generated during analysis.
- `report/` – Detailed findings report.

---

**Author:** tanooja karri

**Skills Demonstrated:** Data Cleaning | EDA | Python | Statistics | Hypothesis Testing | Business Insights
