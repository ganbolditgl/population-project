# 성 및 연령별 추계인구 분석 프로젝트

이 프로젝트는 `성_및_연령별_추계인구.csv` 데이터를 활용하여 성별 및 연령별 장래인구추계 변화를 분석하는 Jupyter Notebook 프로젝트입니다.

## 프로젝트 목적

- 2022년부터 2072년까지의 전체 인구 변화 확인
- 성별 인구 추계 비교
- 선택한 연도의 연령별 인구 구조 시각화
- 특정 연령 구간의 연도별 인구 변화 분석
- wide format 데이터를 long format으로 변환하여 분석하기 쉬운 데이터 구조 만들기

## 파일 구성

```text
.
├── README.md
├── GITHUB_UPLOAD_GUIDE.md
├── requirements.txt
├── 빅데이터프로젝트.ipynb
├── data/
│   └── 성_및_연령별_추계인구.csv
└── outputs/
    └── .gitkeep
```

## 사용 데이터

데이터 파일:

```text
data/성_및_연령별_추계인구.csv
```

주요 열 설명:

| 열 이름 | 설명 |
|---|---|
| 가정별 | 추계 시나리오 |
| 성별 | 성별 구분 |
| 연령별 | 연령 구간 |
| 2022-2072 | 연도별 추계 인구 |

CSV 파일은 한글이 포함되어 있어 `cp949` encoding으로 읽습니다.

## 실행 방법

필요한 Python 라이브러리를 설치합니다.

```bash
pip install -r requirements.txt
```

그 다음 Jupyter Notebook을 실행합니다.

```bash
jupyter notebook
```

Notebook 파일:

```text
빅데이터프로젝트.ipynb
```

## 분석 흐름

1. `pandas`, `matplotlib`, `pathlib` 라이브러리 불러오기
2. CSV 파일을 `cp949` encoding으로 읽기
3. 데이터 구조와 열 이름 확인
4. 열 이름을 분석하기 쉬운 이름으로 변경
5. 전체 인구 추계 데이터 추출
6. 전체 인구 변화 선 그래프 작성
7. 데이터를 long format으로 변환
8. 성별 인구 비교 그래프 작성
9. 선택한 연도의 연령별 인구 막대그래프 작성
10. 특정 연령 구간의 연도별 변화 분석
11. 변환된 데이터를 `outputs/population_long_format.csv`로 저장

## 주요 결과 예시

- 전체 인구는 연도별로 감소하는 추세를 확인할 수 있습니다.
- 성별 인구 추계를 비교하여 남녀 인구 변화 흐름을 확인할 수 있습니다.
- 연령별 막대그래프를 통해 특정 연도의 인구 구조를 한눈에 볼 수 있습니다.

## 사용 기술

- Python
- Pandas
- Matplotlib
- Jupyter Notebook

