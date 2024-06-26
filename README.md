# Imbalance_Handling_PySpark
**불균형 데이터 처리 알고리즘 PySpark 구현 및 심장병 예측\
팀원: 김기수, 배홍섭, 백시관,  정태영\
프로젝트 기간 : 22.11.6~22.12.16**\
**사용 데이터 : 캐글 데이터 셋 이용** https://www.kaggle.com/code/omarmohamedyehia/heart-disease-prediction

# 프로젝트 선정 이유
대부분의 Task에서 라벨 데이터의 불균형 비율이 큰 데이터가 많음.\
일반적인 학부 프로젝트나 학습 및 캐글에서 만나는 데이터의 경우 크기가 작아 Pandas를 이용해도 무방했음.\
이에 따라 대부분 scikit-learn 라이브러리에 존재하는 imbalanced-learn 패키지를 통해 해결이 가능했음.\
참고 : https://github.com/power-TY/ML_TeamProject

그러나 실제 필드에서 이용하는 데이터의 경우 빅데이터로 Pandas로 처리하기에는 여러가지 문제점이 존재함.

**빅데이터의 문제**
1. 데이터 규모의 증가
2. 데이터 규모의 증가로 인한 처리 속도 문제
3. 데이터 포맷의 다양성 증가

PySpark에서는 PySpark DataFrame을 통해 전체 데이터를 메모리에 저장하지 않고 효율적으로 처리할 수 있음.\
\
**하지만 PySpark에는 기존에 진행했던 프로젝트 불균형 데이터에 대한 처리를 진행할 때 이용할 수 있는 라이브러리가 따로 존재하지 않음.**\
이에 따라 기존 프로젝트와 같은 데이터를 PySpark dataframe으로 불러오고 불균형 알고리즘을 구현하여 성능을 비교함.

# 구현 알고리즘
**RandomOverSampling, RandomUnderSampling, SMOTE, BorderlineSMOTE ADASYN, Cost-Sensitive**\
프로젝트 기한 관계상 대부분 가장 많이 이용하고 범용성이 넓은 오버샘플링을 위주로 구현.









