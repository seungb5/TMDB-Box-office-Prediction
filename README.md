![](https://pbs.twimg.com/profile_images/789117657714831361/zGfknUu8_400x400.jpg)
# **TMDB Box Office Prediction**
- [https://www.kaggle.com/c/tmdb-box-office-prediction](https://www.kaggle.com/c/tmdb-box-office-prediction/)

___
## **1. 개요**
TMDB Box Office Prediction :
- [TMDB](https://www.themoviedb.org/)에서 수집한 과거 데이터를 이용하여, 영화의 수익률 예측.
- 문제 유형 : Regression

#### **1.1. 문제 접근 방법**
- 이번 경진 대회에서는 3000개의 학습용 데이터와 4397개의 테스트 데이터를 제공한다. 학습용 데이터의 수가 테스트 데이터보다 부족하다는 문제점을 가진다. 또한 discussion과 kernel을 참고한 결과, 제공된 데이터의 신뢰성에대해 적지 않은 문제점을 식별할 수 있었다. 이는 차후에 모델의 성능 개선을 위해 고려해야 할 사항이다.

0) [변수 정보](https://github.com/seungb5/TMDB-Box-office-Prediction/blob/master/%EB%B3%80%EC%88%98%20%EC%A0%95%EB%B3%B4_python.ipynb)
1) [EDA & FE](https://github.com/seungb5/TMDB-Box-office-Prediction/blob/master/EDA%2C%20FE.ipynb)
2) model 
- [base model](https://www.kaggle.com/tmznql1234/base-model) : 1st submission
- [2nd submission](https://github.com/seungb5/TMDB-Box-office-Prediction/blob/master/seoul-coding-academy_2nd_submission.ipynb)

3)  
- sklearn에서 DecisionTree, RandomForest, ExtraTrees, AdaBoost, GradientBoosting 등 다양한 트리 모델을 지원한다. 그러나 최근에는 XGBoost와 LightGBM을 많이 사용하여 좋은 성과를 내고 있다.
- XGBoost는 가장 좋은 성능과 빠른 속도를 제공하는 트리 모델이며, LightGBM은 마이크로소프트에서 오픈소스로 제공한 Boosting Tree 모델로서, XGBoost보다 빠른 학습 속도와 안정적인 성능을 제공하기 때문에 base 모델로 사용하게 되었다.
___
## **2. 팀 구성**
#### 2.1. **팀원 소개**
| 이름 | 역할 | 
| :------------ | :-----------: | 
| 안 승 보 | Base 모델의 발굴/ 선택/ 작성, 주요 모델 개선 아이디어 수집, 튜닝 | 
| 김 건 모 | Feature engineering 아이디어 제시, 데이터 전처리 및 변환 | 
| 김 다 영 | Discussion을 이용한 정보 습득, 제공된 데이터 이외의 정보 취득| 
| 김 도 민 | kernel 발굴 및 code의 이해와 공유, 비교 모델 개선 아이디어 수집, 튜닝 | 
| 조 수 빈 | 데이터의 Feature 관리, 데이터 시각화를 이용한 결론 도출|

#### 2.2. **팀 운영 방법**
작업 내용 공유:
##### **Google drive를 이용한 공용 드라이브 운영**
![](https://user-images.githubusercontent.com/46778769/56775271-47c72400-6801-11e9-86c2-0d063b14ea23.PNG)
##### **github를 이용한 협업**
![](https://user-images.githubusercontent.com/46778769/56771316-3d9d2980-67f1-11e9-928e-820196dca0cf.PNG)
#####  **github issue를 이용한 code 공유**
![](https://user-images.githubusercontent.com/46778769/56771008-6b35a300-67f0-11e9-9c0c-9516f32a18dd.PNG)