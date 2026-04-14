# 📰 NLP 기초: CountVectorizer를 이용한 뉴스그룹 텍스트 분류

> 데이터관리론 4월 과제 | 2555031 이지원 | 2026.04

---

## 과제 개요

sklearn의 20 Newsgroups 데이터셋을 활용하여 텍스트를 수치화하고, **코사인 유사도**를 통해 새로운 문장이 어떤 주제에 속하는지 분류하는 프로그램을 구현한다.

### 분류 카테고리

| 카테고리 | 주제 |
|---|---|
| `comp.graphics` | 컴퓨터 그래픽 |
| `sci.space` | 우주 과학 |
| `talk.religion.misc` | 종교 토론 |

---

## 파일 구성

| 파일명 | 설명 |
|--------|------|
| `nlp_assignment.ipynb` | 전체 분석 코드 및 고찰 (Colab 노트북) |
| `README.md` | 과제 설명 문서 |

---

## 구현 내용

1. **데이터 수집**: 3가지 주제별 20개 샘플 추출 (총 60개 문서)
2. **전처리**: 헤더, 푸터, 인용구 제거 + 영어 불용어 제거
3. **벡터화**: CountVectorizer로 단어 빈도 기반 벡터 변환
4. **분류**: 코사인 유사도 기반 최근접 문서 매칭
5. **고찰**: OOV 문제 분석 및 성능 개선 실험 (샘플 수 증가 / TF-IDF / bigram)
6. **배포**: Gradio 웹 서비스 구현

---

## 실행 방법

1. `nlp_assignment.ipynb`를 Google Colab에서 열기
2. 런타임 → 모두 실행 (`Ctrl + F9`)

---

## 사용 기술

- **분석 환경**: Google Colab (Python 3)
- **주요 라이브러리**: scikit-learn, numpy, Gradio
