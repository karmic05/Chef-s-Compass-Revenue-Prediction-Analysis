# 🍽️ Chef's Compass Revenue Prediction Analysis

## 📌 Business Problem
Chef's Compass, an innovative meal delivery service, needed to understand the core drivers of customer revenue during their first year. The objective of this project is to predict customer revenue based on behavioral and engagement metrics to help stakeholders optimize marketing spend, improve customer retention strategies, and identify high-value VIP segments. 

## 🛠️ Tech Stack
* **Languages:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-learn (Gradient Boosting, Random Forest, Lasso, Ridge, KNN)
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Google Colab

## 🔬 Methodology
1. **Exploratory Data Analysis (EDA):** Analyzed a dataset of ~2,000 customers and 19 variables. Identified a right-skewed revenue distribution (median $1,740 vs. mean $2,107). 
2. **Data Preprocessing & Feature Engineering:** Handled missing values, cleaned anomalous columns, applied logarithmic transformations to normalize right-skewed data, and extracted email domains to create targetable marketing groups.
3. **Predictive Modeling:** Trained and evaluated multiple regression models, ultimately selecting a **Gradient Boosting Machine (GBM)** for its optimal balance of predictive accuracy and stakeholder interpretability.

## 📊 Key Insights
* **Menu Exploration Drives Revenue:** `UNIQUE_MEALS_PURCH` demonstrated a strong positive correlation with revenue; customers who explore diverse menu options spend significantly more.
* **Engagement is a Strong Predictor:** `CONTACTS_W_CUSTOMER_SERVICE` showed a moderate positive correlation. Highly engaged customers who reach out—even with complaints—represent a higher-value segment.
* **Platform Agnostic Value:** Both Mobile and PC logins positively correlate with revenue, emphasizing the need for a seamless omnichannel experience.

## 💡 Business Recommendations
* Launch targeted retention campaigns specifically for the high-value tail-end of the revenue distribution (customers generating up to $8,794).
* Incentivize new users to try diverse meals to boost their long-term value.
* Prioritize subscription conversion (`WEEKLY_PLAN`) as a primary KPI for first-year retention.
