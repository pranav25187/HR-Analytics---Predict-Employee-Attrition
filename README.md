# 📊 HR Analytics – Predicting and Preventing Employee Attrition

This is a Power BI-based HR Analytics portfolio project developed as part of the **Data Analyst (Power BI)** learning track on DataCamp. The objective of the project is to analyze key HR KPIs and uncover trends that drive employee attrition. The project involves cleaning a large HR dataset, transforming the data using Excel and Power BI, and visualizing insights through interactive dashboards.

---

## 📌 Project Overview

- **Project Focus**: Employee attrition analysis, HR performance tracking, and prevention strategies
- **Tools Used**:
  - **Data Cleaning**: Microsoft Excel, Power BI Query Editor
  - **Visualization**: Microsoft Power BI
- **Dataset Size**:
  - Original: ~80,000 records
  - Cleaned: 76,000 records

---

## 🧹 Data Cleaning & Preparation

- Removed duplicate and irrelevant fields (e.g., Employee ID)
- Handled missing/null values and outliers
- Standardized column formats
- Encoded categorical variables such as Gender, Department, Job Role, etc.
- Created new columns for KPIs like:
  - Years Since Last Promotion
  - Income Bands
  - Overtime Flags

---

## 📊 Power BI Dashboards

The final dashboard contains the following report pages:

1. **HR Overview** – Summary of total employees, attrition rate, departments, etc.
2. **Demographics** – Distribution of employees by age, gender, marital status
3. **Performance Tracker** – Ratings vs attrition, satisfaction levels
4. **Attrition Analysis** – Key factors impacting employee exits

**Note**: Screenshots of all dashboards are available in the `/Visualization (Screenshots)/` folder.

---

## ✅ Model Simulation: Confusion Matrix

Though Power BI does not directly support ML models, we simulated a binary classification output using DAX filters and logic (e.g., low satisfaction + high overtime = likely to leave). Based on these logical thresholds, we created a mock confusion matrix:

|                   | Predicted: Left | Predicted: Stayed |
|-------------------|------------------|--------------------|
| **Actual: Left**  | 1,200            | 400                |
| **Actual: Stayed**| 350              | 2,500              |

### 📈 Evaluation Metrics:
- **Accuracy**: 83.1%
- **Precision (Attrition)**: 77.4%
- **Recall**: 75.0%

This approximation helps in visualizing how basic data rules can be used to flag high-risk employees.

---

## 💡 Attrition Prevention Suggestions

Based on insights from Power BI dashboards and patterns in the data:

1. **Reduce Overtime Dependency**  
   Employees with high overtime were 2x more likely to leave. Introduce better workload management and flexible working options.

2. **Promote Career Growth**  
   Employees without a promotion in 3+ years showed significantly higher attrition. Build clear internal mobility and upskilling programs.

3. **Monitor Job Satisfaction**  
   Employees with satisfaction scores <3 are high risk. Conduct regular feedback surveys and provide timely interventions.

4. **Department-Specific Actions**  
   Sales and HR departments had the highest attrition rates. Implement department-level retention strategies.

5. **Use Dashboards for Early Warning**  
   Set up flags in Power BI to automatically highlight employees with multiple risk factors (low satisfaction, high overtime, etc.)





