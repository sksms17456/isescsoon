---
title: (2주차) 챗봇 만들기!!
---

---
# 인생은 선착순이조 첫 번째 팀!
---

# Career_bot_In_Slack
### # Member
[박현빈](https://github.com/sksms17456) (SAFFY 7반 인생은 선착순이조)
- 채용 파트 : 채용 정보 크롤링(사람인) 및 구현, 일자 입력 받아 찾는 부분 구현
- 오픽 파트 : 크롤링(오픽 홈페이지) 및 구현, 월 입력 받아 찾는 부분 구현  
  
[이기인](https://github.com/marco0332) (SAFFY 7반 인생은 선착순이조)
- 채용 파트 : 크롤링 데이터 정제, 기업 평가 크롤링(잡플래닛) 및 구현
- 토익 파트 : 크롤링(토익 홈페이지) 및 구현
- 오픽 파트 : 크롤링 데이터 정제  
  
[정준태](https://github.com/JunTaeJung) (SAFFY 7반 인생은 선착순이조)  
- 전체 개요 담당
- 발표 파트 담당
- 분위기 메이커♥

### # Requirements
<pre><code>pip install -r requirements.txt</code></pre>

### # How To Use It?    
Career_bot은 키워드로 작동합니다.  
<pre><code>키워드: 채용, 토익, 오픽, 퇴근</code></pre>

![image](https://user-images.githubusercontent.com/27988544/50329806-21843580-053c-11e9-875b-a11c9722c3ac.png)
<br>
<br>
<br>

#### 1. 키워드 '채용'
***  
- 채용이란 단어를 포함시켜서 멘션을 보내게 될 경우, 오늘 시작되는 채용 정보를 출력하게 됩니다.
![image](https://user-images.githubusercontent.com/27988544/50329793-17623700-053c-11e9-8f1f-68ccb19c5b4e.png)

- 특정 날짜를 입력할 경우 그 날에 시작하는 채용정보를 출력합니다.
![image](https://user-images.githubusercontent.com/27988544/50329869-4e384d00-053c-11e9-8721-c5db8c0867e1.png)

- 또한 채용 정보가 출력이 될 때, 각 기업별 평점도 같이 출력됩니다.
![image](https://user-images.githubusercontent.com/27988544/50329901-6a3bee80-053c-11e9-9b4a-ae17a39501cc.png)
<br>
<br>
<br>

#### 2. 키워드 '토익'
***
- 토익 단어를 포함시켜서 멘션을 보내면, 오늘로 부터 가장 시작 일자가 가까운 시험 4개를 출력합니다.
![image](https://user-images.githubusercontent.com/27988544/50330082-46c57380-053d-11e9-8d44-d1db4f8b1bd3.png)
<br>
<br>
<br>

#### 3. 키워드 '오픽'
***
- 오픽 키워드를 입력하면 이번 달에 있는 오픽 정보를 출력합니다.
![image](https://user-images.githubusercontent.com/27988544/50330166-92781d00-053d-11e9-9e52-989d5c4c16b2.png)

- 특정 월 입력 시 해당 월의 시험 정보를 출력합니다.
![image](https://user-images.githubusercontent.com/27988544/50330138-7f654d00-053d-11e9-9b5a-8d78fb5f9aca.png)
  
  
  
---
# 인생은 선착순이조 두 번째 팀!
---
  
# Hello! This Chatbot in Slack
팀원: [최은영](https://github.com/eun02/chat_bot), [강민](https://github.com/zzangkkmin)

## Requirements
- click==6.7
- Flask==0.12.2
- itsdangerous==0.24
- Jinja2==2.9.6  
- MarkupSafe==1.0  
- numpy  
- pyaml==16.9.0  
- PyYAML ==3.12  
- requests-oauthlib==0.8.0  
- requests==2.18.4  
- six==1.10.0  
- slackclient==1.0.2  
- websocket-client==0.37.0  
- Werkzeug==0.12.2  
- beautifulsoup4==4.6.3  


## @Webtoon_bot7
### 개요
네이버 웹툰 정보를 알고싶은 사람에게 추천해주는 Slack 봇  
데이터 크롤링 사이트 => [네이버웹툰]("comic.naver.com") 
### 개발과정
    - Day 1 초안 기획 및 작성 / 신규, 오늘, 요일별 웹툰 크롤링 및 구현
    - Day 2 장르별, 완결, 특정웹툰 검색, 키워드 검색 기능 구현
    - Day 3 세부 조정 및 이미지 출력

#### 가이드라인
    네이버 웹툰 챗봇 Nchat 입니다.
    다음으로 물어보시면 웹툰을 추천해드리겠습니다.
    
    오늘의 추천 웹툰 -> "오늘의 웹툰"
    이달의 신규 웹툰 -> "신규 웹툰"
    [요일] 웹툰 Top 10 ([정렬]) -> "월요일 웹툰 업데이트순"
    [장르] 웹툰 Top 10 ([정렬]) -> "스토리 웹툰 별점순"
    완결 웹툰 Top 10 ([정렬]) -> "완결 웹툰 조회순"
    특정 웹툰 검색 -> "검색 마음의소리"
    키워드 검색 -> "키워드 연애"

    P.S
    [요일] 월, 화, 수, 목, 금, 토, 일
    [장르] 에피소드, 옴니버스, 스토리, 일상, 개그, 판타지, 액션, 드라마, 순정, 감성, 스릴러, 시대극, 스포츠
    [정렬] 업데이트순, 조회순, 별점순, 제목순(장르 웹툰 제외)
    웹툰 검색은 정확한 명칭(띄어쓰기 포함)으로 입력해주십시오.
    키워드 검색은 해당 키워드를 포함한 모든 웹툰을 보여드립니다.        
    
#### 기능
- 오늘의 추천 웹툰
    - 오늘의 날짜 이용, 날짜와 해당 요일의 추천 웹툰 3개 표시
- 신규 웹툰
    - 이달의 신규 웹툰 3개 표시
- 요일별 웹툰
    - 입력 요일과 순서 옵션 이용, 상위 3개 표시
- 장르별 웹툰
    - 입력 장르와 순서 옵션 이용, 상위 3개 표시 
- 완결 웹툰
    - 순서 옵션 이용, 상위 3개 표시
- 특정 웹툰 검색
    - 입력된 특정 웹툰을 딕셔너리 키 안에서 검색
- 키워드 검색
    - 입력된 키워드를 제목 리스트에서 검색
- 기타 
    - 정확하지 않는 검색은 실패 표시
    - 가이드라인 이외 입력은 다시 가이드라인 표시
 
   
## 회고  
크롤링의 어려움, 봇 호출의 반복  
보완계획: 봇 호출의 반복을 제거, 명단 개수 늘리기  
