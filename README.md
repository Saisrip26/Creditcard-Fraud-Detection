# Credit Card Fraud Detection Project

## 📝 Abstract

Credit card fraud presents a significant challenge in the financial sector, especially within banking. Detecting fraudulent transactions is critical to prevent customers from being charged for unauthorized purchases. This project employs machine learning models to predict fraudulent transactions based on transaction features, aiming to enhance fraud detection capabilities and mitigate risk for financial institutions.

## 🔑 Keywords

- **Credit Card Fraud**
- **Financial Sector Challenges**
- **Fraud Detection**

## 🎯 Objective

The objective of this project is to develop a predictive model that accurately identifies fraudulent transactions, thereby reducing risk for financial institutions.

## 📊 Data

The dataset for this project is sourced from Kaggle and contains transactions made by European cardholders. Here are the key details:

- **Total Transactions**: 284,807
- **Features**:
  - **Time**: Seconds elapsed since the first transaction.
  - **Amount**: Transaction amount.
  - **Class**: Fraud indicator (1 for fraud, 0 for non-fraud).

The dataset includes 28 Principal Component Analysis (PCA) components, but only the first 8 PCA components are used for modeling. The data is imbalanced, with many more non-fraudulent (0) transactions compared to fraudulent (1) ones.

## 🖥️ Programming Language

- **Python** is used for implementation.

## 🔧 Data Preprocessing

### Steps:

1. **Feature Selection**: Excluded the `Time` feature due to minimal impact. Only the first 8 PCA components are used.
2. **Handling Imbalanced Data**: Applied techniques such as resampling to address the class imbalance.
3. **Null Values**: Confirmed that the dataset contains no null values.

## 📈 Modeling

### 1. **Logistic Regression**
- **Accuracy**: 0.97635
- **ROC Score**: 0.997
- **Description**: Logistic Regression is suitable for binary classification tasks. It achieved low error rates and demonstrated good performance and interpretability.

### 2. **Support Vector Classifier (SVC)**
- **Accuracy**: 0.97972
- **ROC Score**: 0.992
- **Description**: SVC, a part of the Support Vector Machine (SVM) family, is effective for high-dimensional data. It provided high performance with fewer errors compared to Logistic Regression.

### 3. **Random Forest Classifier**
- **Accuracy**: 0.96621
- **ROC Score**: 0.994
- **Description**: Random Forest is an ensemble method that combines multiple decision trees to improve accuracy and reduce overfitting. It showed slightly higher error rates than the other models.

## 🏆 Conclusion

Among the models evaluated, **Logistic Regression** achieved the highest accuracy of **0.97635** and demonstrated the best performance with minimal error rates. It is recommended for predicting fraudulent transactions effectively.

## 🔮 Future Work

- **Explore Advanced Models**: Investigate other classification algorithms and feature engineering techniques.
- **Incorporate Additional Features**: Consider adding variables such as income levels and education to improve model performance.

## 📚 References

1. [ScienceDirect Article](https://www.sciencedirect.com/science/article/pii/S187705092030065X)
2. [ResearchGate Article](https://www.researchgate.net/publication/336800562_Credit_Card_Fraud_Detection_using_Machine_Learning_and_Data_Science)
3. [IEEE Xplore Paper](https://ieeexplore.ieee.org/document/5159014)
4. [IJSTR Review](http://www.ijstr.org/final-print/oct2019/A-Review-On-Credit-Card-Fraud-Detection-Using-Machine-Learning.pdf)
5. [AIRCConline Paper](https://aircconline.com/csit/papers/vol10/csit101018.pdf)
6. [IJARCCE Paper](https://ijarcce.com/wp-content/uploads/2016/02/IJARCCE-9.pdf)

## 🛠️ Installation and Dependencies

### Required Libraries:
- Python 3.x
- Numpy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

