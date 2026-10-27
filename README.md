# Balázs Margitai

**Full-Stack Developer** · Data & AI

I build internal web applications at the **University of Debrecen, Faculty of
Informatics**, together with the people who use them, and take each one from
the first conversation to deployment and handover. Recent ones: the faculty
admissions website, an environmental monitoring system for 18 field sensors,
and a document-chain auditing system.

Before that I co-founded **Skillion**, an AI study platform that reached
**10,000+ registered users**. Data Science MSc in progress.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-margitai--balazs--cs-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/margitai-balazs-cs)
[![Email](https://img.shields.io/badge/Email-balazsmargitai%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:balazsmargitai@gmail.com)
![Open to new roles](https://img.shields.io/badge/status-open_to_new_roles-2EA043?style=flat-square)

---

## Selected work

### [grounded-qa](https://github.com/mbalazs03/grounded-qa)

*Python · pgvector · multilingual-e5 · Qwen3 (Ollama) · MLflow*

A local RAG system on SQuAD 2.0, built to answer one question: does it know
when not to answer?

**The hard part:** measuring abstention, not just accuracy. Retrieval puts the
correct passage in the top 5 for 95.1% of answerable questions, yet the system
abstains on only 38% of unanswerable ones. Error analysis traced most wrong
answers to the LLM rather than to retrieval.

### [Stroke Risk Analysis](https://github.com/mbalazs03/stroke-risk-analysis)

*R · R Markdown · logistic regression · LDA · random forest*

Predicting stroke from health data: 5,109 patients, of whom only 4.9% had a
stroke. Exploratory analysis first, then logistic regression, LDA and random
forest compared under nested cross-validation.

**The hard part:** with a 5% positive class, a model that never predicts stroke
is already 95% accurate and completely useless. Tuning the decision threshold
instead of accepting the default 0.5 raised the stroke cases the model detects
from 0 to 38 of 74.

### [Rebrickable API Manager](https://github.com/mbalazs03/rebrickable-api-manager)

[![CI status](https://github.com/mbalazs03/rebrickable-api-manager/actions/workflows/ci.yml/badge.svg)](https://github.com/mbalazs03/rebrickable-api-manager/actions/workflows/ci.yml)

*Java 21 · Spring Boot 3.2 · MongoDB 7 · React 19*

Answers "what can I build right now from the bricks I already own?" Owned sets
are merged into one part inventory, then catalogue sets are scored against it and
ranked by completion.

**The hard part:** quantities decide it, not membership. Three 2×4 bricks do not
cover a requirement for eight, so every part contributes `min(owned, required)`.
The upstream API allows one request per second, so the client paces itself, and
the paging calls go through a retry wrapper that honours the server's
`Retry-After` interval instead of guessing a backoff. Part lists are cached per
set, which keeps one page of results from costing hundreds of calls.

---

## Stack

|**Area**|**Tools**|
|---|---|
| **Languages** | TypeScript · Python · Java · SQL · R |
| **Web** | React · Next.js · React Native · Tailwind |
| **Backend** | FastAPI · Flask · Spring Boot · REST |
| **Data** | PostgreSQL · MongoDB · pgvector · pandas · scikit-learn · XGBoost |
| **AI** | RAG · prompt engineering · MLflow · Claude Code · MCP |
| **Delivery** | Docker · GitHub Actions · Nginx · Azure |

---

## Certifications

Every badge links to its verification page.

[![Anthropic Claude Code in Action](https://img.shields.io/badge/Anthropic-Claude_Code_in_Action-D97757?style=flat-square&logo=anthropic&logoColor=white)](https://verify.skilljar.com/c/c65733ac852d)
[![NVIDIA Generative AI with Diffusion Models](https://img.shields.io/badge/NVIDIA-Generative_AI_with_Diffusion_Models-76B900?style=flat-square&logo=nvidia&logoColor=white)](https://learn.nvidia.com/certificates?id=MFLM5iobQlKuCT6q6oJt3g)
[![AZ-900 Azure Fundamentals](https://img.shields.io/badge/AZ--900-Azure_Fundamentals-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)](https://www.credly.com/badges/f04be3f7-6f97-4b4f-a831-699d0418fb24/public_url)
[![DP-900 Azure Data Fundamentals](https://img.shields.io/badge/DP--900-Azure_Data_Fundamentals-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)](https://www.credly.com/badges/6eacebbf-aa12-448c-827a-bed140901347/public_url)
[![Kaggle Pandas](https://img.shields.io/badge/Kaggle-Pandas-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/learn/certification/balzsmargitai/pandas)
[![Kaggle Intro to Machine Learning](https://img.shields.io/badge/Kaggle-Intro_to_Machine_Learning-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/learn/certification/balzsmargitai/intro-to-machine-learning)
[![IT Specialist Java](https://img.shields.io/badge/IT_Specialist-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](https://www.credly.com/badges/301dd53b-dc9e-4736-98cd-99125f3309ea/public_url)
[![IT Specialist Python](https://img.shields.io/badge/IT_Specialist-Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.credly.com/badges/223d4d77-6cb6-4ffc-ba24-70e56aeda81c/public_url)
[![IT Specialist Databases](https://img.shields.io/badge/IT_Specialist-Databases-4479A1?style=flat-square&logo=postgresql&logoColor=white)](https://www.credly.com/badges/61a852ea-dca0-404b-b3aa-1aec5ecd7e15/public_url)
