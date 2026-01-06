# Smart-Inventory-Demand-Forecasting-using-ML


Accurate demand forecasting is essential for effective retail inventory management. Poor forecasts can lead to stockouts, overstocking, increased operational costs, and customer dissatisfaction. This project proposes a machine learning–based demand forecasting framework that predicts future product demand using historical retail data and integrates those predictions into practical inventory decision-making.

The system is built using a Random Forest regression model, chosen for its ability to capture complex and nonlinear demand patterns while remaining interpretable and computationally efficient. To ensure realistic and unbiased evaluation, the model is assessed using time-based cross-validation and out-of-fold (OOF) predictions, preventing data leakage and overfitting.

🎯 Objectives

- Predict product demand accurately using historical retail data

- Reduce inventory issues such as stockouts and overstocking

- Apply time-aware evaluation for real-world forecasting scenarios

- Bridge the gap between demand forecasting and inventory control logic

🧠 Methodology Overview
1. Dataset Description

The dataset contains historical retail transaction and inventory data, including:
``
- Product and store identifiers

- Historical units sold

- Inventory levels

- Pricing and discount information

- Seasonality and promotional indicators

- Time-related information is preserved to support sequential forecasting and proper evaluation.

2. Data Preprocessing

- Handling missing values using statistical imputation

- Encoding categorical features

- Scaling numerical features where required

- Sorting data chronologically to maintain temporal consistency

3. Feature Engineering

To improve predictive performance, several time-series features are created:

- Lag features (previous demand values)

- Rolling statistics (rolling mean and standard deviation)

- Calendar-based features to capture seasonality

These features help the model learn historical demand patterns more effectively.

4. Model Implementation

Model Used: Random Forest Regressor

- Captures nonlinear relationships between demand and influencing factors

- Robust to noise and outliers

- Requires minimal parameter tuning compared to deep learning models

5. Model Evaluation

To simulate real-world forecasting:

- Time-based cross-validation is applied instead of random splitting

- Out-of-fold (OOF) predictions are generated for unbiased performance estimation

- Evaluation Metrics:

- RMSE (Root Mean Squared Error)

- MAE (Mean Absolute Error)

- R² Score

These metrics help assess both accuracy and reliability of the forecasts.

6. Inventory Decision Logic

The predicted demand is further used to support inventory decisions, including:

- Estimating required stock during supplier lead time

- Determining reorder quantities

- Supporting proactive inventory planning

This step demonstrates how forecasting outputs can directly influence operational decisions.

📊 Results Summary

The Random Forest model outperforms baseline forecasting approaches by:

- Reducing prediction error through feature engineering

- Producing stable forecasts under time-based evaluation

- Providing interpretable insights into demand drivers

(Exact metric values can be found in the notebook outputs.)

🛠️ Technologies Used

- Programming Language: Python

- Libraries: Pandas, NumPy, Scikit-learn, Matplotlib

- Model: Random Forest Regression
- 
📄 Research Paper (LaTeX)

The research paper is written entirely in LaTeX and formatted according to the IEEE conference/journal style.

- Paper Title: Smart Inventory Demand Forecasting using Machine Learning

- Paper Format: LaTeX (IEEE style)

- Main File: main.tex

- Compiled Output: Smart-Inventory-Demand-Forecasting-using-ML.pdf

📌 The paper includes problem motivation, literature review, methodology, equations, experimental results, and discussion.
