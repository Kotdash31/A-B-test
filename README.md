# A/B Test: Evaluation of a New Payment Mechanism
### 📌 Project Overview
In this project, I conduct and analyze the results of an A/B test aimed at evaluating the impact of a new payment mechanism on user behavior.

#### Group A (control group) retained the standard payment flow.

#### Group B (test group) was offered a new payment flow.

### 🎯 Goal
To evaluate whether the new payment mechanism positively affects user behavior and decide whether it should be rolled out to all users.

### 📋 Input Data
The analysis is based on the following CSV files:

- groups.csv — user IDs and their group assignment (A or B);

- active_studs.csv — users who were active on the platform during the experiment;

- checks.csv — payment data for users during the test period.

### 📊 Analysis Steps
1. Data loading, merging, and preprocessing;
2. Choosing main metrics (CR, ARPPU);
3. Creating  dataset with main metrics on which impact of the test can be observed;
4. Using proportion Z-test for identifying statistical effect of changing canversion rate in groups;
5. Checking homoscedasticity in groups' samples;
6. Testing the distribution of user groups for normality;
7. Application of Student's T-test for statistical comparison of ARPPU in groups;
8. Significance assessment;
9. Data visualization;
10. Conclusion and final business recommendation.

### ⚙️ Tools & Libraries
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4B8BBE?style=for-the-badge&logo=bookstack&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)

### ✅ Conclusion
Based on the obtained data, I can conclude that the new payment mechanism affected revenue, as the ARPPU differs significantly between groups (p-value < 0.05).
However, since the number of payments does not differ statistically between groups, the changes did not impact the share of paying customers.

Despite a similar share of paying customers, the new mechanism increases both revenue and ARPPU.
Therefore, it is recommended to launch the new payment mechanism with the goal of increasing revenue.
