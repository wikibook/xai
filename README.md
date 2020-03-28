# XAI 실전 연습을 위한 데이터와 예제

XAI 실전 연습을 위한 데이터 예제.

`Jaehyun Ahn` ([sogosonnet@gmail.com](mailto:sogoaonnet@gmail.com))

## 1. 신용대출 분석 데이터(loan)

### 1.1. 데이터 설명

데이터는 loanData.csv에 저장되어 있다. loanData는 19개의 칼럼으로 되어 있으며, 첫 번째 칼럼부터 18번째 칼럼까지는 대출 신청을 위한 사용자 정보가 저장되어 있으며 19번째 칼럼에는 대출 승인 여부가 이진(binary) 형태로 저장되어 있다.

### 1.2. 칼럼 설명

데이터 칼럼이 의미하는 내용은 다음과 같다.

1. id: 고객 아이디
2. gender: 대출 신청자 성별
3. age: 대출 신청자 나이
4. married: 결혼 유무
5. dependents: 가족 수
6. education: 학력
7. self_employed: 자영업 유무
8. business_type: 국세청 기준 대출 신청인 업종 코드
9. applicant_income: 대출 신청인 수입
10. applicant_work_period: 대출 신청인 근무 기간
11. coapplicant_income: 배우자 수입
12. credit_history: 금융서비스(대출) 이용 횟수
13. credit_amount: 대출중인 금액
14. property_area: 주거지 종류(Urban: 도시, Semiurban: 준도시, Rural: 시골)
15. property_type: 주거지 소유 여부(1: 자가, 2: 월세, 3: 전세, 4: 기타)
16. credit_rate: 신용등급
17. loan_amount: 대출 금액
18. loan_term: 대출 상환 기간
19. loan_status: 대출 승인 여부

### 1.3. 기타

8번 칼럼의 국세청 업종 코드는 이곳(https://www.venturein.or.kr/popup/BusinessCode.do)에서 확인할 수 있다.

Copyright(c)2019 Jaehyun Ahn All rights reserved. 

<hr>

## 2. JAFFE 감정분석 데이터(Emotion)

![JAFFE example](http://www.kasrl.org/KA_004.jpg)

JAFFE 감정분석 데이터 중 놀람(SUP)에 대응하는 이미지 한 장.

### 2.1. 데이터 설명

JAFFE(The Japanese Femail Facial Expression) 데이터베이스는 일본인 여성(학생들)의 얼굴 사진과 감정을 정량적인 수치로 표시한 데이터베이스다.

### 2.2. 데이터 다운로드 방법

JAFFE 데이터베이스는 연구 목적으로만 자유롭게 사용될 수 있으며, 각 사용자들은 모두 라이센스에 동의해야 한다. 라이센스에 대한 동의는 [이 링크](http://www.kasrl.org/jaffedb_info.html)에서 하고 다운 받을 수 있다.

위 링크에서 라이센스 사용에 대한 동의를 한 이후 이미지를 다운 받고 "./Ch2.emotion/jaffe"라는 하위폴더에 이미지를 삽입한다.

### 2.3. 칼럼 설명

이미지에 대응하는 데이터 칼럼이 텍스트파일 형태로 저장되어 있다. 텍스트파일은 "./Ch2.emotion/jaffe/jaffe_labels.txt"에 저장되어 있다.

데이터의 첫 번째와 두 번째 행은 이미지에 대한 설명이다. 이후 행에 대하여 각 칼럼별로 의미하는 바는 다음과 같다.

1. id: 이미지 고유값
2. HAP: 행복
3. SAD: 슬픔
4. SUR: 놀람
5. ANG: 분노
6. DIS: 실망
7. FEA: 두려움
8. PIC: 이미지 이름

### 2.4. 기타

JAFFE 이미지 라이센스는 Michel J. Lyons 교수에게 있다. 이미지를 다운받은 사용자들의 이미지 사용에 대한 책임은 전적으로 이용자에게 있음을 고지한다.

Michael J. Lyons, Shigeru Akemastu, Miyuki Kamachi, Jiro Gyoba.
Coding Facial Expressions with Gabor Wavelets, 3rd IEEE International Conference on Automatic Face and Gesture Recognition, pp. 200-205 (1998).

## 3. 단원별 코랩 데이터

구글 코랩(Google Colab)은 브라우저에서 파이썬을 작성하고 실행할 수 있는 클라우드 기반 주피터 노트북 개발 환경입니다. 코랩과 인터넷만 있으면 예제 코드를 직접 따라하고 실행할 수 있습니다.

|단원|내용|URL|
|---|:----:|---:|
|04 |의사 결정 트리|http://bit.ly/391EmTS|
|05| 대리 분석|http://bit.ly/2RNP6zv|
|06| 필터 시각화| http://bit.ly/37M96YV|
|07| LRP| http://bit.ly/37SDpwX|
|08| 실전 분석1: 의사 결정 트리와 XAI| http://bit.ly/2vBcYxB 또는 <br> 현재 Github Repo의 `Ch1.Loan` 참고|
|09| 실전 분석2: LRP와 XAI| 현재 Github Repo의 `Ch2.Emotion` 참고|


