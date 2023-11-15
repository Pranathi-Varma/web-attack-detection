# Web Attack Detection Project

This repository contains the code and documentation for a Web Attack Detection project, focusing on enhancing the security of web applications through proactive identification and mitigation of various vulnerabilities.

## Introduction

In an era of increased digitalization, the reliance on digital technology extends from simple tasks to highly secure payment activities. Service providers bear the responsibility of safeguarding customer privacy and protecting against security vulnerabilities. This project addresses the complexities of managing firewalls and proposes a solution: monitoring web data, detecting anomalies, and guiding servers to take appropriate actions.

## Methodology

### Data
- **Dataset:** Internet traffic records from a university's firewall, sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Internet+Firewall+Data).
- **Attributes:** 65,532 records with 12 attributes, including a categorical target variable "Action" (Allow, Deny, Drop, Reset-Both).

### Preprocessing
- **Null Values:** Checked and handled appropriately.
- **Action Column:** Dropped "Reset-Both" category due to low representation.
- **Dimensionality Reduction:** Removed highly correlated features.
- **Outliers:** Visualized and examined.
- **Data Split:** Divided into training and testing sets.

### Classification Models
1. **Logistic Regression**
   - Utilized for fast and effective classification of linearly separable data.

2. **Naïve Classification using Dummy Classifier**
   - Serves as a baseline for other classifiers and is particularly useful for datasets with class imbalance.

3. **Decision Trees**
   - A supervised machine learning algorithm used for classification and regression.
   - Parameters were tuned for improved accuracy.

### Experiment and Results
- Model accuracies were recorded for Logistic Regression, Naïve Classifier, and Decision Trees.
- A detailed analysis of the confusion matrices and accuracy was conducted for the Decision Tree model with tuned parameters.

### Database
- **Training & Testing Logs:** Confusion matrices and accuracy metrics for both training and testing data.

### Discussion and Comparison
- A comprehensive discussion comparing true positive and false positive values across different models.

## Conclusion

- The dataset was successfully classified into Allow, Deny, and Drop categories.
- Decision Tree with tuned parameters demonstrated the best performance.
- All models achieved high accuracy, emphasizing the significance of the selected features in internet firewall detection.

## Usage

### Prerequisites
- Python 3.x
- Required libraries: [scikit-learn==0.24.2
pandas==1.3.3
numpy==1.21.2
matplotlib==3.4.3
seaborn==0.11.2
]


