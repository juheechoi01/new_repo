# 2024 봄 KUBIG CONTEST - ML 분반 1팀

---

## 팀원

19기 안태림, 임지우

## 팀명 

Je t'aime

## 주제: 소비자 데이터 기반 소비 예측

https://dacon.io/competitions/official/235893/overview/description

## 목표

본 프로젝트의 목표는 소비자 데이터를 통하여 소비량을 예측하는 것이다. 추가적인 목표로 마케팅 분석가의 입장에서 기대에 미치지 못한 최근의 마케팅 캠페인에 대해 문제를 이해하고 데이터 기반 솔루션을 제안하는 것을 설정하였다. 

## 변수

- id : 샘플 아이디
- target : 고객의 제품 총 소비량

- Year_Birth : 고객 생년월일
- Education : 고객 학력
- Marital_status : 고객 결혼 상태
- Income : 고객 연간 가구 소득
- Kidhome : 고객 가구의 자녀 수
- Teenhome : 고객 가구의 청소년 수
- Dt_Customer : 고객이 회사에 등록한 날짜
- Recency : 고객의 마지막 구매 이후 일수
- NumDealsPurchases : 할인된 구매 횟수
- NumWebPurchases : 회사 웹사이트를 통한 구매 건수
- NumCatalogPurchases : 카탈로그를 사용한 구매 수
- NumStorePuchases : 매장에서 직접 구매한 횟수
- NumWebVisitsMonth : 지난 달 회사 웹사이트 방문 횟수
- AcceptedCmp1: 고객이 첫 번째 캠페인에서 제안을 수락한 경우 1, 그렇지 않은 경우 0
- AcceptedCmp2: 고객이 두 번째 캠페인에서 제안을 수락한 경우 1, 그렇지 않은 경우 0
- AcceptedCmp3: 고객이 세 번째 캠페인에서 제안을 수락한 경우 1, 그렇지 않은 경우 0
- AcceptedCmp4: 고객이 네 번째 캠페인에서 제안을 수락한 경우 1, 그렇지 않은 경우 0
- AcceptedCmp5: 고객이 5번째 캠페인에서 제안을 수락한 경우 1, 그렇지 않은 경우 0
- Complain : 고객이 지난 2년 동안 불만을 제기한 경우 1, 그렇지 않은 경우 0
- Response : 고객이 마지막 캠페인에서 제안을 수락한 경우 1, 그렇지 않은 경우 0

## 프로젝트 진행 방식

### 데이터 EDA를 통해서 데이터를 살펴보고 파생 변수를 생성**

- 'Age'
- 'Age_Range'
- 'Days_Customer'
- 'TotalPurchases'
- 'Preferred_Purchase'
- 'RCatalogPurchases'
- 'RStorePurchases'
- 'RWebPurchases'
- 'NumAcceptedCmp'
- 'Kidhome_has'
- 'Teenhome_has'
- 'Pass_Customer'

### 데이터 전처리 과정을 거쳐 최종적으로 사용할 변수 확정

### PyCaret Automl & H2O Automl 통해 모델 선정

### optuna 통해 최적의 파라미터 산출

### 데이터 기반 솔루션 제공을 위한 Clustering 수행