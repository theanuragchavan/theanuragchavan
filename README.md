# Anurag Chavan

**MSc Computer Science (Artificial Intelligence)** · University of Nottingham (2024–2026)
Software engineer. I build AI systems that hold up outside a demo — and I check whether they actually work before I claim they do.

---

## Featured Projects

### 🔍 [Deep-Research Agent Team with a Validated Grounding Evaluator](https://github.com/theanuragchavan/deep-research-grounding-evaluator)
Event-driven multi-agent research pipeline — a planner fans four sub-questions out to parallel async workers, a counter-based fan-in blocks until every result lands, and a writer produces a cited report. The interesting part is the judge: an LLM scoring every claim against its cited source, **required in code to quote the evidence span**, so it cannot approve a claim it can't point at.

Validated it adversarially with typed corruptions and uncorrupted controls. That exercise found **four defects in my own test harness** rather than in the system under test. A human approval gate raised grounding from 75% to 91% *on planted errors*. Profiling caught one blocking call inside the event loop that had silently reduced four workers to single-worker throughput — 3.12x once fixed.

Full write-up, including what it doesn't do, in [`CASE_STUDY.md`](https://github.com/theanuragchavan/deep-research-grounding-evaluator/blob/main/CASE_STUDY.md).

`Python` · `asyncio` · `LlamaIndex Workflows` · `BM25` · `Langfuse`

---

### 🤖 [Behaviour-Aware Adaptive Dialogue System](https://github.com/theanuragchavan/behaviour-aware-hri)
MSc dissertation. A task-oriented dialogue agent that infers five user engagement states from response latency and turn count using a trained gradient-boosting classifier (≈0.85 macro-F1), then adapts its hints, tone and error-recovery in real time. Provider-agnostic multi-LLM fallback chain (Gemini, Llama, Mistral, plus templates) to keep inference off the paid APIs when it doesn't need them. SHAP prosody sub-study under ethics approval.

`Python` · `scikit-learn` · `LLM APIs` · `ROS` · `JSONL`

---

### 📡 [Big Data GPS Clustering — GeoLife](https://github.com/theanuragchavan/big-data-gps-analysis)
Distributed clustering of 11 million GPS points (Microsoft GeoLife) on Databricks / PySpark. Custom MapPartitions-based KMeans, DBSCAN with Haversine feature engineering, spatial partitioning by lat/lon bucket, and a 200-run grid search. Best silhouette: KMeans 0.705 (cycling), DBSCAN 0.695 (cycling).

`PySpark` · `Databricks` · `KMeans` · `DBSCAN` · `Haversine`

---

### 📈 [BSE Algorithmic Trading Agent](https://github.com/theanuragchavan/bse-trading-agent)
Implemented the **Adaptive Aggressive (AA)** trading algorithm in the Bristol Stock Exchange simulator. EMA equilibrium tracking, Smith's Alpha volatility measurement, Newton-Raphson theta adaptation, and aggressiveness feedback rules. Ran 20 controlled experiments (Baseline ±5 vs High-Noise ±25) across 7 trader types; finished first of seven by mean profit.

`Python` · `BSE` · `Algorithmic Trading` · `Newton-Raphson` · `EMA`

---

### 🐦 [Big Tech Twitter NLP](https://github.com/theanuragchavan/twitter-sentiment-bertopic)
End-to-end NLP pipeline over roughly 2.4 million tweets from the January 2023 ChatGPT/Bing moment: RoBERTa sentiment, BERTopic topic modelling, transformer emotion classification, and geospatial mapping comparing public perception across Google, Microsoft and OpenAI.

`PyTorch` · `Hugging Face` · `RoBERTa` · `BERTopic`

---

### 🛍️ [MERN E-Commerce Platform](https://github.com/theanuragchavan/mern-ecommerce-app)
Full-stack e-commerce app with product catalogue, cart, payments, JWT auth, Cloudinary image upload and SMTP notifications. React + Redux frontend, Express/Node backend, MongoDB Atlas, deployed with environment-variable credential management.

`React` · `Redux` · `Node.js` · `Express` · `MongoDB`

---

### ✈️ [British Airways — Forage virtual experience](https://github.com/theanuragchavan/british-airways-data-science)
A [Forage](https://www.theforage.com/) job simulation, not employment. Two parts: web-scraped and sentiment-analysed 1,000+ customer reviews with BeautifulSoup + VADER; predicted flight-booking completion with a Random Forest classifier (82% accuracy). Key drivers: purchase lead time, flight duration, route.

`Python` · `BeautifulSoup` · `scikit-learn` · `VADER` · `Random Forest`

---

## Tech Stack

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

**AI / ML**
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat&logo=huggingface&logoColor=black)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white)

**Big Data**
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat&logo=apachespark&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat&logo=databricks&logoColor=white)

**Web / Full-Stack**
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)

---

## Contact

- Email: anuragchavan21102@gmail.com
- LinkedIn: [linkedin.com/in/theanuragchavan](https://linkedin.com/in/theanuragchavan)
- GitHub: [github.com/theanuragchavan](https://github.com/theanuragchavan)
