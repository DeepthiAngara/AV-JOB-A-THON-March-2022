# DeepthiAngara-AV-JOB-A-THON-March-2022

**Problem:**
Churn Prediction - Whether a customer will churn or not?

We are asked to analyze the past data of the bank and predict whether the customer will churn or not in the next 6 months.

**Approach:**
Classification Models: 
The feature ‘Is_Churn’ is to predict – ‘Whether the customer will churn in next 6 months or not’, it implies classification models are to be used. Correlation between features is observed using mathplotlib.

**Data Cleaning and Preparation**

**Ignore Features:** Features ‘ID’ and ‘Balance’ are ignored as the feature ‘ID’ is 100% unique and ‘Balance’ is 99.99% unique.

**Encoder:** Categorical features ‘Gender’, ‘Income’, ‘Credit_Category’ and ‘Product_Holdings’ are encoded using Label encoder.

**Features Split:** Training data is split into Independent and dependent features

• Independent features - Age, Gender, Income, Vintage, Transaction_Status,
Product_Holdings, Credit_Card, Credit_Category

• Dependent features - Is_Churn

**Preprocessing**

**Transformation:** Independent features are transformed into the value ranging from - 1 to +1 using ‘Standard Scaler’ transformation.

**Normalization:** Independent features are normalized and applied to Quantile Transformer.

**Features Interaction:** Polynomial Feature Interaction is applied on independent features.

**Cross Validation:** K Fold Cross Validation is applied.

**Model Selection:** Various classification models like Decision Tree, Random Forest, Logistic Regression, and Naive Bayes are build. ‘f1_macro’ is the metric used for performance measure.

Surprisingly, data with only ‘Data Cleaning and Preparation’ gave better performance than data with ‘Preprocessing’ on Random Forest and Gaussian Naive Bayes Mode
