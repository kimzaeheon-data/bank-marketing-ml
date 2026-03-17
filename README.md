# Bank Marketing Prediction

정기예금 가입 여부를 예측하는 머신러닝 프로젝트입니다.

## Dataset
UCI Bank Marketing Dataset

## Models
- Logistic Regression
- Random Forest
- XGBoost

## Evaluation Metric
F1 Score

## Baseline Model Result

The baseline model showed high accuracy but poor recall for the positive class due to class imbalance.

Accuracy : 0.89

Class 1 (Subscriber)
Precision : 0.68  
Recall : 0.21  
F1 Score : 0.32

This indicates the model failed to correctly identify many potential subscribers.

## Tech Stack

- Python
- Pandas
- Scikit-learn
- XGBoost
- Matplotlib
  
## Project Structure

bank-marketing-ml
│
├── README.md
└── bank_marketing_prediction.ipynb
