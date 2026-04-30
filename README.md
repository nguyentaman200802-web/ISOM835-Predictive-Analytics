# E-Commerce Supply Chain Optimization: Predicting Fulfillment Delays

**Author:** An Nguyen
**Course:** ISOM 835 – Predictive Analytics and Machine Learning 

## 📌 Project Overview & Objectives
Supply chain bottlenecks are a major cost driver for e-commerce organizations. The objective of this project is to bridge technical machine learning with actionable business strategy by predicting whether a shipment will arrive on time or be delayed. By accurately predicting late deliveries based on leading indicators (like product weight and warehouse routing), operations managers can proactively intervene to prevent fulfillment delays and improve customer satisfaction.

## 🚀 Key Business Insights
Through Exploratory Data Analysis (EDA) and predictive modeling, several critical operational bottlenecks were identified:
* **The 10% Discount "Cliff":** Deep marketing discounts are fundamentally breaking the supply chain. 100% of shipments receiving a discount greater than 10% are delayed. Flash-sale discounts must be capped or coordinated with warehouse capacity.
* **Capacity Overload at Block F:** Warehouse F processes nearly double the volume of any other facility, creating a highly centralized, imbalanced network topology. Immediate load-balancing protocols are recommended to divert inventory to other blocks.
* **The "Lightweight" Penalty:** Counter-intuitively, heavier packages (4,000–6,000 grams) consistently arrive on time, while delayed packages are heavily skewed toward lighter weights (2,000–4,000 grams). This suggests a flaw in sorting procedures where lightweight packages are bulk-processed or deprioritized.

## 📊 Dataset Description
* **Source:** [Kaggle: E-Commerce Shipping Data](https://www.kaggle.com/datasets/prachi13/customer-analytics)
* **Details:** This dataset contains 10,999 observations of international supply chain operations. It captures critical logistical variables such as warehouse block origins, modes of shipment, product weight, customer discount rates, and historical customer ratings.

## 🛠️ Tools & Libraries Used
* **Language:** Python
* **Environment:** Google Colab, GitHub
* **Libraries:** `pandas` (Data manipulation), `matplotlib` & `seaborn` (Data visualization), `scikit-learn` (Machine Learning, Preprocessing, Evaluation)
* **Models Deployed:** Logistic Regression, Random Forest Classifier

## 📈 Model Performance
The models were evaluated on a 20% holdout testing set. The **Random Forest Classifier** outperformed the baseline model, achieving:
* **Accuracy:** 66.32%
* **F1 Score:** 0.6969 (Chosen as the primary metric to balance the business risks of False Positives and False Negatives in logistics).

## 💻 How to Run This Project
All code and analysis were completed in Google Colab. To view the code, visualizations, and model outputs:

1. Click the link below to open the notebook in Google Colab.
2. (https://colab.research.google.com/drive/1TeUmLlwRQIVnRfo4UZ_4MB82Go-ixUoS?usp=sharing)
3. *Note: To run the cells yourself, you will need to download the `Train.csv` file from the Kaggle link above and upload it to the Colab session storage.*

Alternatively, you can read the full, comprehensive analysis in the `Term Project Final Report.pdf` located in the `reports/` folder of this repository.
