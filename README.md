# LG-Aimers 2기
Phase2 과제

**[Dataset Info.]**

**train.csv [파일]**
- PRODUCT_ID : 제품의 고유 ID
- Y_Class : 제품 품질 상태(Target) 
  - 0 : 적정 기준 미달 (부적합)
  - 1 : 적합
  - 2 : 적정 기준 초과 (부적합)
- Y_Quality : 제품 품질 관련 정량적 수치
- TIMESTAMP : 제품이 공정에 들어간 시각
- LINE : 제품이 들어간 공정 LINE 종류 ('T050304', 'T050307', 'T100304', 'T100306', 'T010306', 'T010305' 존재)
- PRODUCT_CODE : 제품의 CODE 번호 ('A_31', 'T_31', 'O_31' 존재)
- X_1 ~ X_2875 : 공정 과정에서 추출되어 비식별화된 변수

**test.csv [파일]**
- PRODUCT_ID : 제품의 고유 ID
- TIMESTAMP : 제품이 공정에 들어간 시각
- LINE : 제품이 들어간 공정 LINE 종류 ('T050304', 'T050307', 'T100304', 'T100306', 'T010306', 'T010305' 존재)
- PRODUCT_CODE : 제품의 CODE 번호 ('A_31', 'T_31', 'O_31' 존재)
- X_1 ~ X_2875 : 공정 과정에서 추출되어 비식별화된 변수


**sample_submission.csv [파일]** - 제출 양식
- PRODUCT_ID : 제품의 고유 ID
- Y_Class : 예측한 제품 품질 상태
- 0 : 적정 기준 미달 (부적합)
- 1 : 적합
- 2 : 적정 기준 초과 (부적합)

실제 공정 과정에서의 데이터로, 보안상의 이유로 일부 변수가 비식별화 처리(X변수)
'LINE', 'PRODUCT_CODE'는 Train / Test 모두 동일한 종류가 존재
