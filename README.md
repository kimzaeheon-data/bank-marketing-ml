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

## Threshold Tuning

To improve recall for the subscriber class, the classification threshold was adjusted.

Baseline threshold : 0.5

After testing multiple thresholds, the optimal threshold was found to be **0.25**.

Result:

Precision : 0.50  
Recall : 0.54  

Lowering the threshold significantly improved the model's ability to identify potential subscribers.

## Model Comparison

| Model | Precision | Recall | F1 Score |
|------|------|------|------|
| Logistic Regression | 0.68 | 0.21 | 0.32 |
| Random Forest | 0.58 | 0.30 | 0.40 |
| XGBoost (baseline) | 0.66 | 0.27 | 0.39 |
| XGBoost (threshold=0.25) | 0.50 | 0.54 | 0.52 |

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
