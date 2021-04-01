# Data analysis & machine-learning
## 1. iris 품종 예측
> sklearn에서 제공하는 데이터셋이기 때문에 간단하게 iris.data, iris.target으로 X,y 값을 나눌 수 있습니다.
> 
> train셋에 overfitting 될 수 있기 때문에 kfold 상세조정을 하여 cross_val_score로 교차검증 준비를 합니다.
> 
> 분류 모델인 knn, decisiontree, randomforest, svm 을 사용하여 교차검증 한 모델의 평균 정확도를 구할 수 있습니다.

## 2. titanic 생존자 예측
> kaggle에서 제공하는 데이터셋이므로 info()를 통해 결측치, 이상치를 확인합니다.
> 
> 결측치가 존재하는 컬럼의 값을 fillna()를 이용해 채워줍니다. (평균치로 채울때는 np.mean())
> 
> 불필요한 컬럼을 drop한 후 label encoding으로 string값을 정수형으로 바꿉니다.
> 
> train 셋에서 가장 높은 정확도를 보인 RandomForestClassifier로 test셋을 예측합니다

## 3. breast cancer, santander 은행 고객 만족 예측
> LightGBM을 사용하여 평가하였습니다.
> 
> Santander 데이터셋 같은 경우 target 값이 불균형하기 때문에 train test 셋을 분리할 때 target값의 비율이 비슷하게 나눠지기 위해 stratify 를 설정하였습니다.
