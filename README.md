
# BCG X Data Science Internship: PowerCo Churn Analysis


##  Project Overview
This project is part of the **BCG X Data Science Virtual Internship**. The objective was to support **PowerCo**, a major energy utility provider, in understanding and mitigating customer churn in the competitive SME (Small & Medium Enterprise) market.

The central business challenge was to test the hypothesis: **"Is customer churn driven by price sensitivity?"** Through exploratory data analysis, advanced feature engineering, and machine learning, I developed a predictive model to identify high-risk customers and provided actionable recommendations to the SME division head.

---

##  Technologies & Tools
* **Language:** Python
* **Libraries:** `Pandas`, `NumPy`, `Scikit-Learn`, `Matplotlib`, `Seaborn`, `Joblib`
* **Modeling:** Random Forest Classifier
* **Techniques:** SMOTE (imbalanced data handling), RFM Analysis, Feature Importance, Hyperparameter Tuning.

---

##  The Data Science Lifecycle

### 1. Business Understanding & Problem Framing
* Defined the "price sensitivity" hypothesis.
* Quantified the impact of churn on PowerCo's revenue.
* Identified the SME segment as the primary focus for retention.

### 2. Exploratory Data Analysis (EDA)
* Analyzed customer consumption patterns, pricing history, and churn rates.
* **Key Finding:** Churn was approximately **10%**, but price sensitivity showed a weak correlation with churn when viewed in isolation, suggesting other factors like tenure and service engagement were at play.

### 3. Feature Engineering
* **Price Delta:** Calculated the difference between off-peak, mid-peak, and peak prices from December to January to capture "sticker shock."
* **Tenure:** Converted date features into "Months of Service."
* **Log Transformation:** Applied to skewed consumption data to improve model stability.
* **Categorical Encoding:** Transformed sales channels and contract types into machine-readable formats.

### 4. Modeling & Evaluation
* Developed a **Random Forest Classifier** to predict the probability of churn.
* **Performance:** Evaluated using Precision, Recall, and ROC-AUC metrics.
* **Result:** The model successfully identified high-risk customers, with **Tenure** and **Yearly Consumption** emerging as stronger predictors than price sensitivity.

### 5. Insights & Recommendations
* **Targeted Retention:** Recommended a **20% discount strategy** exclusively for customers with a >50% churn probability.
* **Proactive Engagement:** Shifted focus from reactive pricing to proactive service improvements for newer customers (the highest risk group).
* **Operationalization:** Provided a serialized model (`.pkl`) for integration into PowerCo’s CRM.

---

##  Key Findings
> "While price sensitivity has some impact, it is not the sole driver of churn. Newer customers and those with specific consumption profiles are at much higher risk, requiring a multi-faceted retention approach beyond just discounts."

---



##  Skills Mastered
* **Hypothesis Development:** Framing data questions to solve business dilemmas.
* **Information Synthesis:** Turning complex model outputs into executive summaries.
* **Mathematical Modeling:** Implementing ensemble methods to solve classification problems.
* **Client Communication:** Bridging the gap between technical data science and management consulting.

