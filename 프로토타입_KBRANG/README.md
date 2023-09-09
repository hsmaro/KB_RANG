# KB RANG (Recommendation system And New Generation)

## 제 5회 Fututre Finance A.I. Challenge

- 주관기관 KB 국민은행

## 생성 AI 모델을 활용한 개인맞춤 경제 뉴스 기사 추천 서비스

- 금융 어플리케이션의 MAU (Monthly Active User) 및 DAU(Daily Active User)를 증가시키기 위해서 컨텐츠 추가 및 하루 한번 접속을 통한 일상 그 자체를 녹여낼 수 있는 컨텐츠 필요
- 생성 모델을 활용한 경제 문제 및 정답 자동 생성
- 생성된 문제를 사용자에게 제공하여 문제의 카테고리별 정답률과 클릭률 및 개인정보(성별, 연령대, 거주지 등)를 통한 개인 맞춤 경제 뉴스 추천 시스템

>  프로토타입 링크 : https://lvbw36rfmca4idskyq6jum.streamlit.app/

## 프로토타입 실행방법

```
cd 프로토타입_KBRANG > cd Streamlit > 
streamlit run main.py
```


## Project 구조

```
├── KBRANG_prototype/
│   ├── Generation Datasets/ # for dataset
│   │   ├── Data Crawling/
│   │   │   └── news_db_crawling.ipynb  # for news crawling
│   │   ├──user_data.ipynb # for generation imitaion user dataset
│   │   └── aihub_ox_data.ipynb # for preprocessing ox data
│   ├── Models
│   │   ├── Generation model/ # for generation
│   │   │   └── GPT_API_GenQ.ipynb # few-shot learning with OPEN API for Generation Dataset
│   │	│   └── kb_albert.ipynb # generation answer with kb-albert
│   │   │   └── kobert.ipynb # generation answer with kobert
│   │	│   └── KoElectra.ipynb # generation answer with KoElectra
│   ├─ Recommendation System/
│   │   └── models/
│   │   │   └── neural_collaborative_filtering.py # collaboraive filtering with NCF model
│   │   └── utils/
│   │       └── preprocessing.py # preprocessing for user dataset
│   └── Streamlit/  # for prototype
│            └── data/
│            └── app.py  # total app flow
│            └── main.py # to run folder
│            └── news.py # for rec sys
│            └── quiz.py # for quiz
│            └── user.py # for user and update user db
│            └── style.css # for decorating
│ 
├── requrirements.txt
└── README.md
```

### Contribute

|Name|NickName|Profile|
|:--|:---|:-----|
|차형석|hsmaro|https://github.com/hsmaro|
|김동하|Eastha0526|https://github.com/Eastha0526|
|권경민|km0228kr|https://github.com/km0228kr|