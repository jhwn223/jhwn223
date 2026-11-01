<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=3000&pause=800&color=F59E0B&center=true&vCenter=true&width=600&height=60&lines=Hi%2C+I+am+Jihwan+(Juan)+Kim;School+of+Software+%40+CAU;Aspiring+Data+Scientist;Data+for+better+decisions" alt="Typing SVG" />

**School of Software, Chung-Ang University** 🎓 &nbsp;·&nbsp; Seoul, South Korea

I'm interested in using **statistics and data to support better decisions**,
and I plan to pursue a graduate degree in data science.

[![Portfolio](https://img.shields.io/badge/Portfolio-F59E0B?style=for-the-badge&logo=googlechrome&logoColor=white)](https://jhwn223.github.io) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jihwan-juan-kim-12b15740b/) [![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kimjh050223@gmail.com)

</div>

---

## 🛠 Skills

| | |
|:---|:---|
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Java](https://img.shields.io/badge/Java_(coursework)-007396?style=flat-square&logo=openjdk&logoColor=white) ![C](https://img.shields.io/badge/C_(coursework)-A8B9CC?style=flat-square&logo=c&logoColor=black) |
| **Data Analysis** | ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) ![PyArrow](https://img.shields.io/badge/PyArrow-FF6F00?style=flat-square&logo=apachearrow&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square) |
| **Machine Learning** | ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![Model Evaluation](https://img.shields.io/badge/Model_Evaluation-2E8B57?style=flat-square) ![Calibration](https://img.shields.io/badge/Calibration-6C7A89?style=flat-square) ![Feature Engineering](https://img.shields.io/badge/Feature_Engineering-8E44AD?style=flat-square) |
| **Tools** | ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white) |

---

## 💡 Personal Projects

*Self-directed data science projects, currently in progress.*

### 🧠 Facial Expression Model Audit ![In Progress](https://img.shields.io/badge/In_Progress-F59E0B?style=flat-square)

An external audit of a public Hugging Face facial expression model (`trpakov/vit-face-expression`) without retraining. The initial 22.6% accuracy turned out to be driven largely by a preprocessing mismatch in the evaluation pipeline, not the model itself.

- Changing only the input crop raised accuracy from **22.6% → 45.3%**, with non-overlapping 95% CIs
- Reproducible audit pipeline: bootstrap CIs, calibration (ECE, Brier), FDR correction, tests, and a Streamlit dashboard
- Documented the remaining gap vs. the model card and explicit usage limitations

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

🔗 [Project page](https://jhwn223.github.io/projects/facial-expression-audit/) · [Repository](https://github.com/jhwn223/facial-expression-analysis)

<br/>

### 🚲 Ttareungi — Predicting Bike Shortages in Seoul's Public Bike System ![In Progress](https://img.shields.io/badge/In_Progress-F59E0B?style=flat-square)

Diagnosing and predicting station-level bike shortages using 1.7M rental records (Jan 2025) combined with weather data.

- Shortages concentrate at weekday 7 AM; OD analysis shows bikes serve as a last-mile link to subway stations
- Random Forest with lag and weather features improved AUC from **0.66 → 0.73** over a logistic regression baseline

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![PyArrow](https://img.shields.io/badge/PyArrow-FF6F00?style=flat-square&logo=apachearrow&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

🔗 [Project page](https://jhwn223.github.io/projects/ttareungi/) · [Repository](https://github.com/jhwn223/ttareungi-project)

---

## 🏆 Competition & Club Projects

*Web projects built for a competition and a university club's industry project program.*

#### ⚽ MatchplanXI — 2026 World Cup Tactics Simulator

`Competition entry`

A web simulator where you manage any of the 48 national teams from the group stage to the final, then compare your results with the real tournament.

- Drag-and-drop squad builder with 8 formations and role-based auto-placement
- Custom **altitude conditioning index** based on venue altitude, rest days, and recent minutes
- 2D animated match engine with half-time tactical changes

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white) ![dnd-kit](https://img.shields.io/badge/dnd--kit-2C3E50?style=flat-square) ![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat-square&logo=framer&logoColor=white)

🔗 [Live Demo](https://jhwn223.github.io/MatchplanXI/) · [Repository](https://github.com/jhwn223/MatchplanXI)

<br/>

#### 🗺 Coursepic — Plan a Date Course Together with One Invite Link

`University club industry project`

A collaborative web MVP for planning date courses with friends or partners. No sign-up needed: join a shared room with a nickname and an invite link.

- Real-time sync of places, participants, and comments via Supabase Realtime
- Propose-and-approve editing flow when two or more people are in a room
- Participant-level access control with Row Level Security and PostgreSQL RPC

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Kakao Maps](https://img.shields.io/badge/Kakao_Maps-FFCD00?style=flat-square&logo=kakao&logoColor=black) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

🔗 [Live Demo](https://travel-szul.vercel.app)

---

## 📚 Currently Learning

### LIKELION — Data Analysis with SQL, Python & Tableau

`Aug 2026 –` &nbsp;·&nbsp; A hands-on course covering a practical analytics workflow from SQL to Python to Tableau. Notes and exercises will be uploaded to a repository.

![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)

<!-- To be added after the semester starts
### Machine Learning
`Sep 2026 –`

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
-->
