# E-Commerce Supply Chain Optimization: Predicting Fulfillment Delays

**Author:** An Nguyen
**Course:** ISOM 835 – Predictive Analytics and Machine Learning 

## 📌 Project Overview & Objectives
[cite_start]Supply chain bottlenecks are a major cost driver for e-commerce organizations[cite: 29]. [cite_start]The objective of this project is to bridge technical machine learning with actionable business strategy by predicting whether a shipment will arrive on time or be delayed[cite: 26, 28]. [cite_start]By accurately predicting late deliveries based on leading indicators (like product weight and warehouse routing), operations managers can proactively intervene to prevent fulfillment delays and improve customer satisfaction[cite: 30].

## 🚀 Key Business Insights
Through Exploratory Data Analysis (EDA) and predictive modeling, several critical operational bottlenecks were identified:
* [cite_start]**The 10% Discount "Cliff":** Deep marketing discounts are fundamentally breaking the supply chain[cite: 56]. [cite_start]100% of shipments receiving a discount greater than 10% are delayed[cite: 55]. [cite_start]Flash-sale discounts must be capped or coordinated with warehouse capacity[cite: 107].
* [cite_start]**Capacity Overload at Block F:** Warehouse F processes nearly double the volume of any other facility, creating a highly centralized, imbalanced network topology[cite: 41, 42]. [cite_start]Immediate load-balancing protocols are recommended to divert inventory to other blocks[cite: 96].
* [cite_start]**The "Lightweight" Penalty:** Counter-intuitively, heavier packages (4,000–6,000 grams) consistently arrive on time, while delayed packages are heavily skewed toward lighter weights (2,000–4,000 grams)[cite: 46, 47]. [cite_start]This suggests a flaw in sorting procedures where lightweight packages are bulk-processed or deprioritized[cite: 50].

## 📊 Dataset Description
* [cite_start]**Source:** [Kaggle: E-Commerce Shipping Data](https://www.kaggle.com/datasets/prachi13/customer-analytics) [cite: 24]
* [cite_start]**Details:** This dataset contains 10,999 observations of international supply chain operations[cite: 25]. [cite_start]It captures critical logistical variables such as warehouse block origins, modes of shipment, product weight, customer discount rates, and historical customer ratings[cite: 25].

## 🛠️ Tools & Libraries Used
* **Language:** Python
* **Environment:** Google Colab, GitHub
* **Libraries:** `pandas` (Data manipulation), `matplotlib` & `seaborn` (Data visualization), `scikit-learn` (Machine Learning, Preprocessing, Evaluation)
* [cite_start]**Models Deployed:** Logistic Regression [cite: 82][cite_start], Random Forest Classifier [cite: 80]

## 📈 Model Performance
[cite_start]The models were evaluated on a 20% holdout testing set[cite: 86]. The **Random Forest Classifier** outperformed the baseline model, achieving:
* [cite_start]**Accuracy:** 66.32% [cite: 88]
* [cite_start]**F1 Score:** 0.6969 [cite: 91] [cite_start](Chosen as the primary metric to balance the business risks of False Positives and False Negatives in logistics [cite: 89, 90]).

## 💻 How to Run This Project
All code and analysis were completed in Google Colab. To view the code, visualizations, and model outputs:

1. Click the link below to open the notebook in Google Colab.
2. ** (https://colab.research.google.com/drive/1TeUmLlwRQIVnRfo4UZ_4MB82Go-ixUoS?usp=sharing) **
3. *Note: To run the cells yourself, you will need to download the `Train.csv` file from the Kaggle link above and upload it to the Colab session storage.*

Alternatively, you can read the full, comprehensive analysis in the `Term Project Final Report.pdf` located in the `reports/` folder of this repository.
