Here's a refined and GitHub-ready `README.md` file for the African disaster analysis, complete with images integrated as described:

---

# Disaster Aftermath Analysis: Africa

## Overview
This section presents our in-depth analysis of disaster impact on African countries, focusing on predictive modeling and data transformation techniques to assess disaster outcomes across the continent. Through exploratory data analysis (EDA), model comparison, and clustering, we derive insights into the severity, frequency, and financial implications of disasters in Africa.

### Key Highlights:
1. **Dataset**: Data extracted from DesInventar provides disaster metrics across African nations, including Tunisia, Senegal, Uganda, and Tanzania.
2. **Objective**: To predict mortality and financial loss per disaster using Elastic Net and Random Forest Regression, with a specific emphasis on discovering high-risk zones and understanding the influence of disaster frequency and severity.

---

## Data Preprocessing
1. **Data Cleaning**:
   - Removed duplicate entries and standardized missing data handling, maintaining less than 5% NaN values for robust model input.
   - Transformed all event names to uppercase for consistency and readability.

     ![image](https://github.com/user-attachments/assets/49e3443c-9dce-4e69-a075-5dbd348eb61b)


2. **Feature Engineering**:
   - Consolidated loss indicators into `Monetary_LossUSD` by combining local and USD losses.
   - Merged directly and indirectly affected populations for a unified `Affected` variable.
   - Created `Event_Severity` based on the ratio of deaths to event records, adjusting values to ensure relative comparability.

---

## Visualization
Africa's disaster dataset was visualized at both country and continent levels to highlight severity trends and major event types across the region.

### 1. Comparison Plot
The comparison plot showcases the distribution of events and the frequency of high-severity cases across Tunisia, Senegal, and other nations.

### 2. Heatmaps
Heatmaps depict high-impact zones, marking regions experiencing repeated or severe events for further investigation.

![image](https://github.com/user-attachments/assets/61004e57-cbd0-4566-a18c-c467c6f163e6)

---

## Modeling and Analysis

### Regression Models

1. **Elastic Net Regression**:
   - Africa achieved modest accuracy in predicting deaths with Elastic Net, indicating some limitations due to model responsiveness in Tunisia and Senegal.
   - Accuracy: Elastic Net (25%) vs. Random Forest (73.5%).

2. **Random Forest**:
   - Performed consistently better for Africa, achieving an accuracy of 73.5% in predicting death counts.
   - Best suited for capturing non-linear patterns in the African dataset.


---

### Cluster Analysis
Using K-Medoids clustering, we classified disaster risk levels across African nations based on key indicators:

1. Clusters were formed around mortality rates, `Monetary_LossUSD`, and affected populations.
2. Key insights:
   - Countries like Tunisia experienced clustering in higher-risk zones.
   - Incident frequency (DataCards) correlated inversely with mortality, suggesting that areas with fewer but severe events may require more focused intervention.

![image](https://github.com/user-attachments/assets/44e1635a-9658-4135-bb3a-b55d5c196082)

---

## Insights and Action Plan

- **Policy Recommendations**:
  - Improved response frameworks for high-severity clusters identified in Tunisia and Senegal.
  - Targeted resource allocation to minimize disaster impacts in identified risk zones.

- **Future Directions**:
  - Integrate temporal analysis for trends over time, enabling more proactive disaster preparedness.
  - Refine model selection to improve prediction accuracy for high-risk countries in Africa.

)

---

## Conclusion
The analysis provides essential insights for managing and mitigating disaster impact across African countries by combining predictive modeling, clustering, and data visualization. This GitHub repository contains all necessary data, models, and visualizations to support further exploration and proactive disaster management efforts in Africa.

--- 

