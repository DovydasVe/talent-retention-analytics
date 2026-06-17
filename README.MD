# ABS Tech HR Analytics: Talent Retention & Turnover Prediction

A data-driven HR analytics and predictive modeling project designed for **ABS Tech** to analyze employee attrition, define a multi-dimensional "talent" classification, predict flight-risk probabilities among high-performing employees, and deliver strategic recommendations to HR leadership.

---

## 📂 Repository Structure

*   [ABS Tech Case 2026_Data.xlsx](file:///c:/Users/dovyd/OneDrive/Desktop/University/Year%202/HR%20analytics/ABS%20Tech%20Case%202026_Data.xlsx) – Raw Excel sheet containing employee metadata, performance reviews, demographic information, and engagement surveys.
*   [Cleaned_ABS_Tech_Case_2026_Data.xlsx](file:///c:/Users/dovyd/OneDrive/Desktop/University/Year%202/HR%20analytics/Cleaned_ABS_Tech_Case_2026_Data.xlsx) – The preprocessed and standard-scaled dataset ready for statistical tests and modeling.
*   [Preprocessing.py](file:///c:/Users/dovyd/OneDrive/Desktop/University/Year%202/HR%20analytics/Preprocessing.py) – Automated Python script to clean categorical text columns and scale numerical features using `StandardScaler`.
*   [Turnover_analysis.ipynb](file:///c:/Users/dovyd/OneDrive/Desktop/University/Year%202/HR%20analytics/Turnover_analysis.ipynb) – Jupyter notebook examining macro turnover trends over time, self-reported exit reasons, and statistical hypothesis testing (e.g., t-tests/chi-square) to find features significant to attrition.
*   [Talent_analysis.ipynb](file:///c:/Users/dovyd/OneDrive/Desktop/University/Year%202/HR%20analytics/Talent_analysis.ipynb) – Jupyter notebook establishing a weighted formula to calculate a composite **Talent Score** (based on technical, personal, and interpersonal aspects) and analyzing recruitment sources.
*   [Predictive_model.ipynb](file:///c:/Users/dovyd/OneDrive/Desktop/University/Year%202/HR%20analytics/Predictive_model.ipynb) – Machine learning notebook implementing a Logistic Regression pipeline with balanced class weights and Stratified 5-Fold cross-validation (achieving ~87.3% accuracy). Evaluates flight risk for active talents and compares steady vs. high-risk talent characteristics.
*   [Final report.pdf](file:///c:/Users/dovyd/OneDrive/Desktop/University/Year%202/HR%20analytics/Final%20report.pdf) – Comprehensive executive report presenting methodology, results, risk metrics, and mitigation strategies.
*   [HR presentation.pdf](file:///c:/Users/dovyd/OneDrive/Desktop/University/Year%202/HR%20analytics/HR%20presentation.pdf) – Stakeholder presentation deck mapping out insights, high-risk sectors, and retention tactics.

---

## 📈 Methodology & Analytical Pipeline

1.  **Data Preprocessing & Scaling**: Normalized features such as survey responses, absences, training hours, and performance scores using `StandardScaler` to ensure unbiased learning.
2.  **Talent Definition (Feature Engineering)**: Developed a weighted formula categorized as follows:
    *   **Technical Score** (45%): Technical Level, Training Hours, AI Use/Confidence, Innovation, Special Projects.
    *   **Personal Score** (25%): Performance, Engagement, Work-life Balance, Job Stress.
    *   **Interpersonal Score** (30%): Feedback & Trust, Teamwork, Networking, Colleague Assessment.
3.  **Statistical Validation**: Performed feature significance testing on attributes showing strong correlations with volunteer terminations.
4.  **Predictive Modeling**: Trained a classifier to identify flight risk probabilities, allowing HR to proactively address talent retention in specific critical sectors.
