# Credit_Risk-Analysis
### Project Summary: Credit Risk Analysis Using Machine Learning

#### 1. **Business Problem Overview**
   - **Objective**: To analyze and predict credit risk for a bank's customers using internal data and external credit ratings provided by CIBIL, a leading credit rating agency.
   - **Importance**: Effective credit risk assessment is crucial for minimizing the risk of defaults and making informed lending decisions. This project aims to enhance the bank's decision-making process by utilizing advanced machine learning techniques.

#### 2. **Data Collection and Preparation**
   - **Data Sources**: 
      - **Internal Bank Data**: Customer transaction history, demographic information, and previous loan details.
      - **External CIBIL Data**: Credit scores, credit history, and ratings from the CIBIL database.
   - **Data Cleaning**: 
      - Missing values were addressed using imputation methods or by removing incomplete records.
      - Outliers were identified and handled to prevent skewed results.
   - **Data Merging**: 
      - The bank’s customer data was merged with the CIBIL dataset to create a comprehensive view of each customer's credit risk profile.

#### 3. **Exploratory Data Analysis (EDA)**
   - **Statistical Tests**:
      - **ANOVA (Analysis of Variance)**: Used to determine if there are statistically significant differences between the means of various customer groups based on different features.
      - **Chi-Square Test**: Applied to assess the relationship between categorical features, such as customer demographic information and loan repayment status.
   - **Multicollinearity Check**:
      - **Variance Inflation Factor (VIF)**: Conducted to detect multicollinearity among features, ensuring that redundant variables were identified and removed to improve model performance.

#### 4. **Feature Selection and Engineering**
   - **Elimination of Non-Important Features**:
      - After statistical analysis and multicollinearity checks, non-contributory or redundant features were eliminated to streamline the model and reduce overfitting risks.
   - **Feature Engineering**:
      - New features were created based on domain knowledge and data insights to improve the predictive power of the models.

#### 5. **Data Splitting**
   - **Training and Testing Sets**:
      - The cleaned and refined dataset was split into training (70%) and testing (30%) sets to evaluate model performance on unseen data.
      - Stratified sampling was used to ensure that both sets had a balanced distribution of the target variable.

#### 6. **Model Training and Selection**
   - **Algorithms Used**:
      - **Balanced Random Forest**:
         - A variation of the Random Forest algorithm, it is particularly effective in handling imbalanced datasets by balancing the class distribution during the training process. It works by under-sampling the majority class and over-sampling the minority class, ensuring that the model does not favor the majority class.
      - **Decision Tree**:
         - A simple yet powerful algorithm that splits the dataset into subsets based on feature values, creating a tree-like model of decisions. It's interpretable and handles both categorical and numerical data, making it useful for understanding the key factors influencing credit risk.
      - **Random Forest**:
         - An ensemble learning method that constructs multiple decision trees and merges their results to improve accuracy and avoid overfitting. It’s robust to noise and can handle large datasets with higher dimensionality.
      - **Boosting Techniques (e.g., XGBoost, AdaBoost)**:
         - These algorithms work by combining the predictions of multiple weak learners (usually decision trees) to create a strong learner. Boosting sequentially adjusts the weights of incorrect predictions to minimize the overall error, making it highly effective for improving model accuracy.

#### 7. **Model Evaluation**
   - **Accuracy Achieved**: 
      - The models were evaluated on the test dataset, and the Balanced Random Forest achieved the highest accuracy of 98.75%, demonstrating its effectiveness in predicting credit risk.
   - **Predicted Features**:
      - The model successfully predicted key risk indicators (P1, P2, P3, and P4) based on the customer’s previous transactions and credit history.

#### 8. **Outcome and Business Impact**
   - **Result Sharing**:
      - The results, including the risk predictions and the most influential features, were shared with the bank's business team.
   - **Next Steps**:
      - The insights derived from the model will be used to refine the bank’s credit approval process, offering a more data-driven approach to credit risk management.

This detailed summary captures the key aspects of the project, from data preparation to model training, and outlines the significance of each step in achieving the project’s objectives.
