<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=3000&pause=800&color=F59E0B&center=true&vCenter=true&width=600&height=60&lines=Hi%2C+I+am+Jihwan+Kim;Software+Engineering+%40+CAU;Studying+Data+Science+%26+ML;Always+building+something" alt="Typing SVG" />

**중앙대학교 소프트웨어학부** 🎓 &nbsp;·&nbsp; Seoul, South Korea


[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kimjh050223@gmail.com) [![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/jhwn223) [![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/j_hwn._k/) [![Portfolio](https://img.shields.io/badge/Portfolio-F59E0B?style=for-the-badge&logo=googlechrome&logoColor=white)](https://jhwn223.github.io)

</div>

---

## 🛠 Skills

| | |
|:---|:---|
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white) ![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black) |
| **Data Analysis** | ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) ![PyArrow](https://img.shields.io/badge/PyArrow-FF6F00?style=flat-square&logo=apachearrow&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square) |
| **Machine Learning** | ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![Model Evaluation](https://img.shields.io/badge/Model_Evaluation-2E8B57?style=flat-square) ![Calibration](https://img.shields.io/badge/Calibration-6C7A89?style=flat-square) ![Feature Engineering](https://img.shields.io/badge/Feature_Engineering-8E44AD?style=flat-square) |
| **Backend & DB** | ![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Realtime](https://img.shields.io/badge/Realtime-3FCF8E?style=flat-square) ![Row Level Security](https://img.shields.io/badge/Row_Level_Security-4169E1?style=flat-square) |
| **Tools** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white) ![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![npm](https://img.shields.io/badge/npm-CB3837?style=flat-square&logo=npm&logoColor=white) |
| **Deploy** | ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white) ![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?style=flat-square&logo=githubpages&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) |

---

## 🚀 Projects

### 🧠 Facial Expression Model Analysis — 공개 모델 감사, 그리고 감사 방법론의 함정

Hugging Face의 얼굴 표정 분류 모델(`trpakov/vit-face-expression`)을 **새로 학습하지 않고** 외부 데이터에서 검증한 프로젝트입니다. 처음 측정값은 Accuracy 22.6%였지만, 원인을 추적한 결과 그 숫자의 절반 이상이 모델이 아니라 **평가 파이프라인의 전처리 불일치**에서 온 것임을 밝혔습니다.

- **원인 분리 실험** — 체크포인트·표본 939장·지표 구현을 모두 고정하고 **입력 크롭만** 변경. 장면 전체를 넣으면 Accuracy 22.6% (95% CI 20.3–24.8), 얼굴 영역만 잘라 넣으면 **45.3%** (42.7–47.7). Macro F1은 0.134 → 0.302로 2.3배, 두 조건의 신뢰구간은 겹치지 않음
- **오귀속 차단** — 낮은 점수를 모델 탓으로 돌리기 전에 라벨 오정렬 가능성을 먼저 배제. 7개 클래스의 모든 재배치를 탐색해 최적 할당으로도 +5.9%p에 그침을 확인
- **붕괴의 정체** — 모든 정답 클래스가 `sad` 하나로 몰리던 현상(전체의 61.6%)은 모델의 편향이 아니라 프레이밍 산물. 크롭 후 40.4%로 감소하고 최빈 클래스가 `happy`로 전환
- **남은 격차의 정직한 보고** — 정렬 후에도 45.3%로 모델 카드의 71.16%에 미달. `disgust`는 두 조건 모두 F1 0.000, `surprise`는 Precision 0.923 / Recall 0.100. 전처리로 설명되지 않는 잔여 실패를 구분해 기록
- **신뢰도** — ECE 40.7%p → 34.8%p, Brier 1.074 → 0.865로 개선되었으나 평균 신뢰도가 80.1%까지 함께 상승해 과신은 유지. 원점수를 정답 확률로 해석할 수 없음
- **재현 가능한 감사 파이프라인** — 고정 리비전, 계층화 부트스트랩 CI, Wilson 구간, 15-bin ECE, BH FDR 보정, 산출물 무결성 검증, pytest·ruff·Streamlit 대시보드
- **사용 제한 명시** — 원본 얼굴 미배포, 인구통계 추정 없음, 채용·법 집행·감시 등 의사결정 용도 사용 금지. 성능 개선은 배포 근거가 아님을 결론에 명시

**핵심 교훈** — 공개 모델 감사에서 보고되는 낮은 외부 성능은 모델과 평가 설계의 결합 효과이며, 입력 조건을 통제하지 않으면 파이프라인의 결함이 모델의 결함으로 오귀속됩니다.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

🔗 [Repository](https://github.com/jhwn223/facial-expression-analysis)

<br/>

### ⚽ MatchplanXI — 2026 월드컵 전술 시뮬레이터

48개국 대표팀을 직접 운영하며 조별리그부터 토너먼트까지 치러보는 웹 시뮬레이터입니다. 실제 대회 일정과 선수 데이터를 기반으로 전술을 짜고, 경기 결과를 실제 기록과 비교합니다.

- **드래그 앤 드롭 스쿼드 관리** — 8가지 포메이션, 역할 기반 자동 배치, 수비/밸런스/공격 프리셋
- **고도 적응 지수(altitude conditioning index)** — 경기장 고도·휴식일·최근 출전 시간·A매치 출전 수를 반영한 자체 지표
- **2D 애니메이션 경기 진행** — 실시간 전개, 골 연출, 하프타임 전술 조정, 교체 5카드 제한
- **실제 결과 비교** — 경기 후 실제 대회 기록과 나란히 비교

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white) ![dnd-kit](https://img.shields.io/badge/dnd--kit-2C3E50?style=flat-square) ![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat-square&logo=framer&logoColor=white)

🔗 [Live Demo](https://jhwn223.github.io/MatchplanXI/) · [Repository](https://github.com/jhwn223/MatchplanXI)

<br/>

### 🗺 Coursepic — 로그인 없이 초대 링크 하나로 함께 만드는 데이트 코스

연인이나 친구가 같은 코스 방에 모여 장소를 찾고, 의견을 나누고, 코스를 함께 완성하는 협업형 웹 MVP입니다. 회원가입 대신 닉네임과 익명 세션을 쓰고, 초대 링크를 받은 사람은 곧바로 같은 방의 코스와 대화를 실시간으로 봅니다.

- **익명 참여와 공유방** — 로그인 없이 닉네임으로 입장, 초대 코드 링크·카카오톡 공유로 같은 방 진입, 현재 참여자와 편집 상태 실시간 표시
- **카카오맵 장소 탐색** — 키워드·카테고리 검색, 검색 결과와 코스 장소를 지도 마커로 표시, 상세 정보 확인 후 코스 후보로 추가
- **인원에 따라 갈리는 편집 규칙** — 1명이면 즉시 반영, 2명 이상이면 제안 → 다른 참여자의 수락·거절을 거쳐 반영. 중복 추가·중복 제안 방지
- **실시간 동기화** — Supabase Realtime으로 코스 장소, 참여자, 댓글, 제안 상태를 모든 화면에 동시 반영
- **접근 제어** — Row Level Security와 PostgreSQL RPC로 코스 참여자 단위 권한 관리
- **모바일 작업 화면** — 하단 코스·지도·대화 탭 전환, 장소 카드 드래그로 방문 순서 변경, 반응형 레이아웃

**다음 확장 범위** — 자동 코스 추천, 길찾기, 전체 거리·예상 시간 계산, 예약·결제, 커뮤니티

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Kakao Maps](https://img.shields.io/badge/Kakao_Maps-FFCD00?style=flat-square&logo=kakao&logoColor=black) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

🔗 [Coursepic 바로가기](https://travel-szul.vercel.app)

<br/>

### 🌐 Portfolio Site

GitHub Pages로 배포한 개인 포트폴리오 페이지입니다.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

🔗 [jhwn223.github.io](https://jhwn223.github.io) · [Repository](https://github.com/jhwn223/jhwn223.github.io)

---

## 🌱 진행 중인 프로젝트

### 🚲 따릉이 프로젝트 — 서울시 공공자전거 부족 예측 ![In Progress](https://img.shields.io/badge/In_Progress-F59E0B?style=flat-square)

서울시 따릉이 대여 기록 170만 건(2025년 1월)과 기상청 날씨 데이터를 결합해 **부족 진단 → 이동 흐름 분석 → 부족 예측** 세 단계로 풀어가는 데이터 분석 프로젝트입니다.

- **부족 진단** — 2,000여 개 대여소의 시간별 순유출입 집계, 평일 오전 7시 출근 시간대에 부족 집중
- **이동 흐름(OD) 분석** — 상위 20개 이동 패턴 추출, 따릉이가 지하철역과 주거·상업 지역을 잇는 **라스트 마일** 수단임을 확인
- **부족 예측** — "시간당 3대 이상 부족" 이진 분류. 로지스틱 회귀 베이스라인 → 시차(lag) 피처와 날씨를 더한 랜덤 포레스트로 **AUC 0.66 → 0.73**
- **가설 검증** — 강수 시 부족 비율 6.9% → 4.5%로 감소

**다음 단계** — 1개월치 데이터의 계절성 한계 보완, 다중 관측소 날씨 데이터 반영, 클래스 불균형에 따른 정밀도 개선

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![PyArrow](https://img.shields.io/badge/PyArrow-FF6F00?style=flat-square&logo=apachearrow&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

🔗 [Repository](https://github.com/jhwn223/ttareungi-project)

---

## 📚 공부 중

### 멋쟁이사자처럼 — 쿠팡 일잘러의 비밀 도구: SQL·Python·Tableau로 끝내는 데이터 분석

`2026.08 ~` &nbsp;·&nbsp; 실무 데이터 분석 워크플로우를 SQL → Python → Tableau 순서로 익히는 과정입니다.
배운 내용과 실습은 저장소에 정리해 올릴 예정입니다.

![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)

<!-- 개강 후 추가 예정
### 머신러닝
`2026.09 ~`

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

### Spring Boot
`2026.09 ~`

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
-->
