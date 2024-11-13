# Credit Card Fraud Detection

This project is a machine learning solution to detect fraudulent credit card transactions. Due to the highly imbalanced nature of the dataset, special techniques were employed to enhance the model's ability to detect fraud. The project leverages **Synthetic Minority Over-sampling Technique (SMOTE)** to balance the dataset and uses **Random Forest** as the primary classifier, achieving high accuracy and reliability in fraud detection.

## Project Overview
- **Goal**: Build a model to accurately detect fraudulent transactions while handling class imbalance.
- **Dataset**: [Credit Card Fraud Detection Dataset from Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Techniques Used**: SMOTE for class imbalance, Random Forest classifier, hyperparameter tuning with Grid Search.

## Project Steps
1. **Data Exploration and Preprocessing**  
   - Analyzed the dataset to understand the distribution and identify class imbalance.
   - Scaled features for better model performance.

2. **Handling Class Imbalance**  
   - Applied SMOTE only on the training set to generate synthetic samples of the minority class (fraudulent transactions).
   - Ensured data integrity by avoiding data leakage through careful application of SMOTE.

3. **Model Training and Tuning**  
   - Trained a Random Forest model and evaluated initial performance.
   - Used Grid Search to optimize hyperparameters (e.g., `n_estimators`, `max_depth`, `min_samples_split`) and improve the F1-score.

4. **Model Evaluation**  
   - Assessed model performance on an imbalanced test set, using key metrics:
     - **Confusion Matrix**
     - **Precision, Recall, and F1-score**
   - Achieved an F1-score of 0.83 on the fraud class, balancing high accuracy with the ability to detect fraud effectively.

## Results
- **Confusion Matrix**  
  The model achieved a balanced performance with a small number of false positives and false negatives:
