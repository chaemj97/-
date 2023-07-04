# 현재 최고 점수
titanic_2.ipynb : 0.8091407011

## titanic_1.ipynb
로지스틱 회귀 사용
from sklearn.linear_model import LogisticRegression
모델 평가 AUC : 0.792292490118577

파일명 : sub_logisticRegression.csv
score : 0.7533106134

## titanic_2.ipynb
로지스틱 회귀 사용
import statsmodels.api as sm
1. 결과를 0과 1로 분류
(결과 1개 차이남)
모델 평가 AUC : 0.792292490118577

파일명 : sub_logistic_sm.csv
score : 0.7513875365

2. 결과를 소수 그대로
모델 평가 AUC : 0.8665349143610013

파일명 : sub_logistic_sm_float.csv
score : 0.8091407011

## titanic_3.ipynb
데이터 불균형 해소를 위한 데이터 증강 (SMOTE) + DecisionTreeClassifier
모델 평가 AUC : 0.7968379446640316

파일명 : sub_smote_DecisionTree.csv
score : 0.7742210321

## titanic_4.ipynb
SMOTE + 4개 모델(로지스틱, 랜덤포레스트, 의사결정나무, xgboost)
가장 성능 좋은 xgboost 선택
모델 평가 AUC : 0.8715083798882681

파일명 : sub_smote_xgboost.csv
score : 0.7500243427