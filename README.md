# 📈 유명 게스트 출현 유튜브 채널 조회수 예측 모델
<br/>

## 🧑‍💻 프로젝트 개요  
유명 게스트 출현 기반 유튜브 채널의 **게스트 정보 및 영상 특성**을 활용하여 **조회수를 예측**하는 것을 목표로 진행되었습니다. 특히 개인의 브랜드 파워 특성을 추가한다며 모델의 예측 성능을 향상시킬 수 있을 것이라는 가설을 세웠으며, 결과적으로 **9~18%의 오차 감소**를 달성했습니다.  
<br/><br/>

## 📦 데이터셋
- **데이터 수집**:  
  - Python 크롤링을 활용해 YouTube 채널의 메타데이터 수집 (조회수, 게스트, 영상 시간 등)
  - 게스트 정보 수작업 입력: 직업군, 나이대, 성별, 브랜드 파워(상, 중, 하) 
<br/>

## 🛠️ 모델 학습 상세 설명
- **최종 사용 모델**: `Ridge`

- **학습 방법**:  
  - 수집한 유튜브 메타데이터를 기반으로 데이터 전처리 
  - **게스트 직업, 업로드 요일, 영상 길이 등 영상 특성**과 **브랜드 파워 지표**를 feature로 구성  
  - 상관관계 분석 및 EDA 후 회귀 모델 적용
  - MSE을 활용한 모델간 예측 성능 평가, 변수 중요도 파악
  - 최종 모델 선정 및 조회수 예측 
<br/>

## 🧩 주요 역할 및 프로젝트 진행 내용
- 유튜브 채널 메타데이터 수집 및 정제
- **EDA 및 특성 간 상관관계 분석**
- **회귀 모델 학습 및 성능 평가** (LinearRegression, Ridge 등)
- **브랜드 파워 특성 반영**을 통한 성능 향상 기여 (예측 오차 최대 18% 감소)
<br/>

## 🛠️ 사용 기술 스택
- Python
- scikit-learn  
- pandas, numpy, matplotlib, seaborn, Selenium  
<br/>

## 🎯 Result
- 더 상세하고 다양한 특성과의 EDA는 코드 결과 및 포트폴리오에서 확인 가능합니다.
<br/>

**조회수와 feature 간의 상관관계**:
- 상관관계가 전반적으로 낮음
- 조회수가 발생한 이후 시청자의 반응(좋아요, 댓글)과 관계된 특성을 제외한다면 **브랜드 파워가 가장 강한 상관 관계**를 가지고 있음
- 유명인이 게스트로 출현하는 만큼 개인의 사회적 영향력과 인지도가 가장 중요한 특성으로 보임  
<img width="1155" height="804" alt="image" src="https://github.com/user-attachments/assets/5b513a6c-521d-409b-816b-b7422635130f" />
<br/><br/><br/>

**브랜드 파워와 조회수와의 관계**

<img width="420" height="400" alt="image" src="https://github.com/user-attachments/assets/eb90a81a-ec85-4552-87d6-bf0934a382dc" />  <img width="420" height="400" alt="image" src="https://github.com/user-attachments/assets/1794798f-1404-4f55-a5d8-616b36f7cab8" />
<br/><br/><br/>

**예측 결과**

<img width="628" height="607" alt="image" src="https://github.com/user-attachments/assets/1468f4d2-0ec7-40a1-8851-50955b64a590" />

