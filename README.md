# 🛍️고객데이터 기반 성별 예측 모델

### 0. 파일구조<br>
├── data/<br>
│   ├── X.csv<br>
│   └── y.csv<br>
├── customer_gender_prediction.ipynb<br>
└── README.md

### 1. 프로젝트 소개
백화점 고객의 1년간의 구매 데이터를 기반으로 고객의 성별을 예측 모델을 만드는 프로젝트입니다

### 2. 사용데이터
데이터 출처 : 한국데이터산업진흥원 빅데이터분석기사 실기 공개 예시 문항

### 3. 주요 기능
   - 데이터 전처리
     데이터 전처리 과정에선 결측치 처리, 인코딩, 스케일링을 적용했습니다
   - 4가지 모델
     Logistic Regression, Decision Tree, RandomForest, XGBoost를 사용해 성능을 비교하였습니다
     RandomizedSearchCV를 이용해 최종 모델을 선정하였습니다

### 4. 결과
   최종 선택 모델 : RandomForest
   4가지 모델의 초기 정확도가 비슷해 RandomizedSearchCV를 이용해 CrossValidation을 진행하였습니다
   CrossValidation 결과, 약  65%의 정확도를 달성하며, RandomForest가 최적 모델임을
   확인했습니다.
