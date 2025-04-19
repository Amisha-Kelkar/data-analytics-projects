The project focuses on predicting customer conversion outcomes using a synthetic digital marketing dataset. The dataset includes customer-level information such as campaign type, delivery channel, ad spend, click-through rates, and conversion behavior. The goal is to build robust classification models to predict whether a user will convert based on these features.
1. **Data Preparation & Feature Engineering**:
Extensive preprocessing was performed including handling missing values, encoding categorical variables (One-Hot & Label Encoding), and scaling numerical features. Website traffic and engagement metrics were also engineered to enrich model inputs.
2. **Class Imbalance Handling**:
Given the skewed distribution of the target variable (Conversion), techniques such as class weighting were applied to prevent model bias and improve predictive performance on the minority class.
3. **Models Trained**:
    1. Logistic Regression
    2. Decision Tree Classifier
    3. Random Forest
    4. XGBoost
  Multiple models were trained and fine-tuned to identify the optimal approach for conversion prediction.
4. **Evaluation Metrics**:
Model performance was assessed using a range of metrics including:
    1. Accuracy
    2. Precision & Recall
    3. F1-Score
    4. Confusion Matrix
  These helped measure both overall performance and class-level predictive capability.
5. **Results & Insights**:
Ensemble models such as Random Forest and XGBoost performed best, especially in handling class imbalance and generalizing across varying campaign strategies. The models highlighted key predictors like Campaign Type, Ad Spend, and Click-Through Rate as critical drivers of conversion.
