# Портфолио проектов — Data Science / ML Engineering

## О себе

Junior Data Scientist / ML Engineer с фокусом на прикладной ML, RAG, LLM-приложения, NLP и production-like ML-сервисы.  
В проектах работал с табличными, текстовыми и мультимодальными данными, классическим ML, embeddings, hybrid search, LLM orchestration, Streamlit-интерфейсами, API-слоем, Docker и базовыми MLOps-подходами.

## Основной стек

**ML / DS:** Python, Pandas, NumPy, scikit-learn, CatBoost, LightGBM, XGBoost, Optuna, SHAP  
**NLP / LLM / RAG:** LangChain, LangGraph, embeddings, BM25, ChromaDB, Transformers, multilingual-e5, LLM API  
**Backend / MLOps:** FastAPI, Docker, PostgreSQL, Kafka, SQLAlchemy, Streamlit, pytest  
**Data:** SQL, OpenPyXL, CSV/Excel processing, feature engineering, model evaluation

---

## Избранные проекты

### 1. RAG-сервис для интеллектуального поиска по корпоративному Excel-реестру

**Тип:** internship / commercial project  
**Направление:** RAG, LLM, semantic search, hybrid retrieval, tabular data  
**Стек:** Python, Pandas, OpenPyXL, LangChain, ChromaDB, BM25, embeddings, Streamlit, LLM API

Прототип сервиса интеллектуального поиска по корпоративному Excel-реестру проектной информации.  
Система обрабатывает табличные данные, превращает строки и связи между сущностями в структурированные документы, выполняет гибридный поиск и формирует ответ с опорой на найденные источники.

**Что реализовано:**

- парсинг Excel-реестра и подготовка структурированных документов;
- обработка листов, строк, метаданных и связей между объектами;
- гибридный поиск: BM25 + vector search;
- reranking с учётом идентификаторов, аббревиатур и смысловой близости;
- генерация grounded answers с привязкой к найденным источникам;
- Streamlit-интерфейс для поиска и анализа результатов.

**Почему проект важен:**  
Проект показывает не только работу с ML/LLM, но и умение собирать прикладной AI-сервис вокруг реальной бизнес-задачи: обработка корпоративных данных, retrieval, генерация ответа, интерфейс и контроль опоры на источники.

---

### 2. CV Analyzer — анализ ИИ-компетенций по резюме и GitHub

**Репозиторий:** [cv-analyzer-gazprom-neft](https://github.com/KsyLight/cv-analyzer-gazprom-neft)  
**Направление:** NLP, HRTech, ML application, candidate scoring  
**Стек:** Python, Streamlit, Transformers, XLM-RoBERTa, PostgreSQL, Docker, GitHub API

HRTech-сервис для анализа резюме и GitHub-профиля кандидата по матрице ИИ-компетенций.  
Приложение оценивает соответствие кандидата AI/DS-ролям, показывает сильные и слабые стороны, формирует рекомендации и предоставляет HR-интерфейс для просмотра заявок.

**Что делал:**

- участвовал в разработке ML-сервиса;
- дообучал модель для анализа компетенций;
- разрабатывал Streamlit-интерфейс;
- занимался докеризацией и настройкой сервера;
- участвовал в проработке продуктовой логики решения.

**Результат:**  
1-е место в ML case-чемпионате «ProЦифру».

**Почему проект важен:**  
Это не просто учебный ноутбук, а полноценный ML-продукт: есть модель, пользовательский сценарий, HR-интерфейс, серверная часть, Docker и командный результат в кейс-чемпионате.

---

### 3. Multi-Agent Interview Coach

**Репозиторий:** [ITMO_megaschool_case_3](https://github.com/KsyLight/ITMO_megaschool_case_3)  
**Направление:** LLM agents, LangGraph, AI application  
**Стек:** Python, LangGraph, Streamlit, GigaChat API, Pydantic

Мультиагентное LLM-приложение для симуляции технического собеседования.  
Система анализирует профиль кандидата, задаёт вопросы, проверяет ответы через отдельного fact-checking агента и формирует финальный отчёт с обратной связью.

**Что реализовано:**

- мультиагентная архитектура Intake / Interviewer / Fact-Checker / Reporter;
- маршрутизация сценария через LangGraph State Graph;
- Streamlit-интерфейс;
- логирование интервью;
- финальный отчёт с оценкой ответов и рекомендациями.

**Почему проект важен:**  
Проект демонстрирует работу с LLM orchestration, агентной архитектурой и построением прикладного AI-сценария вокруг пользовательского процесса.

---

### 4. Real-Time Fraud Detection System

**Путь:** [mts-data-analysis-school/ml-ops-2](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml-ops-2)  
**Направление:** MLOps, fraud detection, streaming ML  
**Стек:** Python, Kafka, PostgreSQL, CatBoost, Streamlit, Docker

Production-like система для потокового определения мошеннических транзакций.  
Архитектура включает генерацию транзакционных событий, передачу через Kafka, ML-сервис для расчёта fraud-score, сохранение результатов в PostgreSQL и Streamlit-интерфейс для мониторинга.

**Что реализовано:**

- потоковая обработка событий;
- ML-скоринг транзакций;
- хранение результатов в PostgreSQL;
- визуальный мониторинг через Streamlit;
- контейнеризированная архитектура.

**Почему проект важен:**  
Проект показывает переход от обучения модели в ноутбуке к сервисной архитектуре: события, скоринг, база данных, мониторинг и контейнеризация.

---

### 5. RAG-пайплайн по PDF-документу

**Путь:** [mts-data-analysis-school/nn3](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn3)  
**Направление:** RAG, document retrieval, local LLM  
**Стек:** Python, LangChain, Chroma, BM25Retriever, EnsembleRetriever, multilingual-e5, Ollama

Учебный RAG-пайплайн для поиска и ответов по PDF-документу.  
Проект включает разбиение текста, построение индекса, retrieval, объединение разных поисковых подходов и генерацию ответа на основе найденного контекста.

**Что реализовано:**

- загрузка и обработка PDF;
- разбиение текста на фрагменты;
- построение векторного индекса;
- BM25 + semantic retrieval;
- EnsembleRetriever;
- генерация ответа через локальную LLM.

**Почему проект важен:**  
Показывает понимание базовых компонентов RAG: chunking, embeddings, retriever, vector store, keyword search и grounded generation.

---

### 6. NLP Salary Prediction

**Путь:** [mts-data-analysis-school/nn1](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn1)  
**Направление:** NLP, text regression  
**Стек:** Python, PyTorch, Transformers, TF-IDF, scikit-learn

Проект по прогнозированию зарплаты на основе текстовых описаний вакансий.  
Используются текстовые признаки, baseline-модели и нейросетевые подходы для решения задачи регрессии.

**Что реализовано:**

- обработка текстов вакансий;
- построение baseline-моделей;
- работа с NLP-признаками;
- сравнение подходов;
- оценка качества регрессии.

**Почему проект важен:**  
Проект показывает работу с неструктурированными текстовыми данными и применение NLP-подходов в прикладной задаче.

---

### 7. Image Preference Prediction

**Путь:** [mts-data-analysis-school/nn2](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn2)  
**Направление:** Computer Vision, multimodal embeddings  
**Стек:** Python, PyTorch, CLIP, CatBoost, embeddings

Проект по определению более предпочтительного изображения из пары.  
Используются эмбеддинги изображений из CLIP и последующая ML-модель для классификации.

**Что реализовано:**

- извлечение image embeddings;
- использование предобученной CLIP-модели;
- обучение классификатора поверх эмбеддингов;
- сравнение качества моделей.

**Почему проект важен:**  
Проект показывает работу с предобученными мультимодальными моделями и комбинацию deep learning embeddings с классическим ML.

---

### 8. Stacking Models with Uncertainty Estimation

**Путь:** [mts-data-analysis-school/ml3](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml3) / [portfolio](https://github.com/KsyLight/portfolio)  
**Направление:** classical ML, ensembles, uncertainty estimation  
**Стек:** Python, scikit-learn, CatBoost, LightGBM, XGBoost, Optuna, SHAP

Проект по построению ансамбля регрессионных моделей с оценкой неопределённости предсказаний.  
Используются несколько boosting-моделей и линейная модель в качестве meta-learner.

**Что реализовано:**

- preprocessing pipeline;
- обучение CatBoost, LightGBM, XGBoost, RandomForest и Ridge;
- stacking ensemble;
- подбор гиперпараметров;
- оценка неопределённости предсказаний;
- анализ доверия к результатам модели.

**Почему проект важен:**  
Хороший классический DS-проект: ансамбли, метрики, интерпретация и анализ устойчивости предсказаний.

---

### 9. Fraud Detection Classification

**Путь:** [mts-data-analysis-school/ml1](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml1)  
**Направление:** classical ML, fraud detection, binary classification  
**Стек:** Python, Pandas, CatBoost, Optuna, SHAP, scikit-learn

Проект по выявлению мошеннических транзакций.  
Включает анализ транзакционных данных, feature engineering, обучение модели классификации, подбор гиперпараметров и оценку качества.

**Что реализовано:**

- обработка транзакционных данных;
- генерация временных и категориальных признаков;
- обучение CatBoostClassifier;
- подбор гиперпараметров через Optuna;
- оценка качества по метрикам классификации;
- интерпретация факторов через SHAP.

**Почему проект важен:**  
Проект демонстрирует полный цикл classical ML-задачи: данные, признаки, модель, метрики и интерпретация.

---

### 10. FastAPI Seller & Books Project

**Путь:** [mts-data-analysis-school/mts-shad-fastapi-project](https://github.com/KsyLight/mts-data-analysis-school/tree/main/mts-shad-fastapi-project)  
**Направление:** backend for ML, API basics  
**Стек:** Python, FastAPI, SQLAlchemy, JWT, SQLite, pytest

Backend-проект на FastAPI с авторизацией, CRUD-операциями, SQLAlchemy, SQLite и тестами.  
Не является ML-проектом напрямую, но хорошо дополняет MLE-портфолио, потому что показывает понимание API-слоя и серверной разработки.

**Что реализовано:**

- REST API на FastAPI;
- работа с базой данных через SQLAlchemy;
- JWT-аутентификация;
- CRUD-операции;
- тесты на pytest.

**Почему проект важен:**  
Для MLE важно не только обучать модели, но и понимать, как упаковывать функциональность в API и интегрировать её в сервис.

---

## Дополнительные проекты

| Проект | Путь | Краткое описание |
|---|---|---|
| Rent Price Regression | `mts-data-analysis-school/ml2` / `portfolio` | Прогнозирование стоимости аренды жилья с CatBoost, Optuna и SHAP. |
| Scrapy Film Parser | `mts-data-analysis-school/wiki-films-scrapy-project` | Парсер фильмов с сохранением данных в CSV. |
| Route Planner | `case-hack-projects/route-project` | Проект по построению маршрутов с использованием графовых алгоритмов. |

---

# Project Portfolio — Data Science / ML Engineering

## About

Junior Data Scientist / ML Engineer focused on applied ML, RAG, LLM applications, NLP and production-like ML services.  
My projects include tabular, text and multimodal data, classical ML, embeddings, hybrid search, LLM orchestration, Streamlit interfaces, API development, Docker and basic MLOps practices.

## Core Stack

**ML / DS:** Python, Pandas, NumPy, scikit-learn, CatBoost, LightGBM, XGBoost, Optuna, SHAP  
**NLP / LLM / RAG:** LangChain, LangGraph, embeddings, BM25, ChromaDB, Transformers, multilingual-e5, LLM API  
**Backend / MLOps:** FastAPI, Docker, PostgreSQL, Kafka, SQLAlchemy, Streamlit, pytest  
**Data:** SQL, OpenPyXL, CSV/Excel processing, feature engineering, model evaluation

---

## Featured Projects

### 1. RAG Search Service for a Corporate Excel Registry

**Type:** internship / commercial project  
**Area:** RAG, LLM, semantic search, hybrid retrieval, tabular data  
**Stack:** Python, Pandas, OpenPyXL, LangChain, ChromaDB, BM25, embeddings, Streamlit, LLM API

A prototype of an intelligent search service for a corporate Excel-based project registry.  
The system processes tabular data, converts rows and entity relations into structured documents, performs hybrid retrieval and generates answers grounded in retrieved sources.

**Implemented:**

- Excel registry parsing and structured document generation;
- processing of sheets, rows, metadata and entity relations;
- hybrid retrieval: BM25 + vector search;
- reranking based on identifiers, abbreviations and semantic similarity;
- grounded answer generation with source references;
- Streamlit interface for search and result analysis.

**Why it matters:**  
The project demonstrates not only ML/LLM skills, but also the ability to build an applied AI service around a real business scenario: corporate data processing, retrieval, answer generation, UI and source-grounded responses.

---

### 2. CV Analyzer — AI Competency Assessment from CV and GitHub

**Repository:** [cv-analyzer-gazprom-neft](https://github.com/KsyLight/cv-analyzer-gazprom-neft)  
**Area:** NLP, HRTech, ML application, candidate scoring  
**Stack:** Python, Streamlit, Transformers, XLM-RoBERTa, PostgreSQL, Docker, GitHub API

An HRTech service for analyzing a candidate's CV and GitHub profile against an AI competency matrix.  
The application estimates candidate-role fit for AI/DS positions, highlights strengths and weaknesses, generates recommendations and provides an HR interface for reviewing applications.

**My contribution:**

- participated in ML service development;
- fine-tuned a model for competency analysis;
- developed parts of the Streamlit interface;
- worked on Docker deployment and server setup;
- contributed to the product logic of the solution.

**Result:**  
1st place in the “ProЦифру” ML case championship.

**Why it matters:**  
This is not just a training notebook, but a full ML product: model, user scenario, HR interface, server-side components, Docker and a team result in a case championship.

---

### 3. Multi-Agent Interview Coach

**Repository:** [ITMO_megaschool_case_3](https://github.com/KsyLight/ITMO_megaschool_case_3)  
**Area:** LLM agents, LangGraph, AI application  
**Stack:** Python, LangGraph, Streamlit, GigaChat API, Pydantic

A multi-agent LLM application for simulating a technical interview.  
The system analyzes a candidate profile, asks interview questions, verifies answers through a separate fact-checking agent and generates a final feedback report.

**Implemented:**

- multi-agent architecture: Intake / Interviewer / Fact-Checker / Reporter;
- scenario routing through a LangGraph State Graph;
- Streamlit interface;
- interview logging;
- final report with answer evaluation and recommendations.

**Why it matters:**  
The project demonstrates LLM orchestration, agent-based architecture and the ability to build an applied AI workflow around a user-facing scenario.

---

### 4. Real-Time Fraud Detection System

**Path:** [mts-data-analysis-school/ml-ops-2](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml-ops-2)  
**Area:** MLOps, fraud detection, streaming ML  
**Stack:** Python, Kafka, PostgreSQL, CatBoost, Streamlit, Docker

A production-like system for real-time fraud transaction detection.  
The architecture includes transaction event generation, Kafka streaming, an ML scoring service, PostgreSQL storage and a Streamlit monitoring interface.

**Implemented:**

- streaming event processing;
- ML scoring for transactions;
- result storage in PostgreSQL;
- visual monitoring with Streamlit;
- containerized architecture.

**Why it matters:**  
The project shows a transition from training a model in a notebook to a service-oriented ML architecture: events, scoring, database, monitoring and containerization.

---

### 5. RAG Pipeline over a PDF Document

**Path:** [mts-data-analysis-school/nn3](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn3)  
**Area:** RAG, document retrieval, local LLM  
**Stack:** Python, LangChain, Chroma, BM25Retriever, EnsembleRetriever, multilingual-e5, Ollama

A training RAG pipeline for search and question answering over a PDF document.  
The project includes text chunking, index building, retrieval, combining different search methods and generating answers based on retrieved context.

**Implemented:**

- PDF loading and processing;
- text splitting into chunks;
- vector index creation;
- BM25 + semantic retrieval;
- EnsembleRetriever;
- answer generation with a local LLM.

**Why it matters:**  
The project shows an understanding of core RAG components: chunking, embeddings, retriever, vector store, keyword search and grounded generation.

---

### 6. NLP Salary Prediction

**Path:** [mts-data-analysis-school/nn1](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn1)  
**Area:** NLP, text regression  
**Stack:** Python, PyTorch, Transformers, TF-IDF, scikit-learn

A project for predicting salary from vacancy text descriptions.  
It uses text features, baseline models and neural approaches to solve a regression task.

**Implemented:**

- vacancy text processing;
- baseline model training;
- NLP feature extraction;
- comparison of different approaches;
- regression quality evaluation.

**Why it matters:**  
The project demonstrates work with unstructured text data and the application of NLP methods to an applied prediction task.

---

### 7. Image Preference Prediction

**Path:** [mts-data-analysis-school/nn2](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn2)  
**Area:** Computer Vision, multimodal embeddings  
**Stack:** Python, PyTorch, CLIP, CatBoost, embeddings

A project for predicting the preferred image from a pair of images.  
It uses image embeddings from CLIP and a downstream ML classifier.

**Implemented:**

- image embedding extraction;
- use of a pretrained CLIP model;
- training a classifier on top of embeddings;
- comparison of model quality.

**Why it matters:**  
The project demonstrates the use of pretrained multimodal models and a combination of deep learning embeddings with classical ML.

---

### 8. Stacking Models with Uncertainty Estimation

**Path:** [mts-data-analysis-school/ml3](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml3) / [portfolio](https://github.com/KsyLight/portfolio)  
**Area:** classical ML, ensembles, uncertainty estimation  
**Stack:** Python, scikit-learn, CatBoost, LightGBM, XGBoost, Optuna, SHAP

A project focused on building an ensemble of regression models with uncertainty estimation.  
Several boosting models and a linear meta-learner are used to build a stacking ensemble.

**Implemented:**

- preprocessing pipeline;
- CatBoost, LightGBM, XGBoost, RandomForest and Ridge training;
- stacking ensemble;
- hyperparameter tuning;
- prediction uncertainty estimation;
- analysis of confidence in model predictions.

**Why it matters:**  
A strong classical DS project: ensembles, metrics, interpretability and prediction robustness analysis.

---

### 9. Fraud Detection Classification

**Path:** [mts-data-analysis-school/ml1](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml1)  
**Area:** classical ML, fraud detection, binary classification  
**Stack:** Python, Pandas, CatBoost, Optuna, SHAP, scikit-learn

A project for detecting fraudulent transactions.  
It includes transaction data analysis, feature engineering, classification model training, hyperparameter tuning and quality evaluation.

**Implemented:**

- transaction data preprocessing;
- generation of temporal and categorical features;
- CatBoostClassifier training;
- hyperparameter tuning with Optuna;
- evaluation with classification metrics;
- feature interpretation with SHAP.

**Why it matters:**  
The project demonstrates a full classical ML workflow: data, features, model, metrics and interpretation.

---

### 10. FastAPI Seller & Books Project

**Path:** [mts-data-analysis-school/mts-shad-fastapi-project](https://github.com/KsyLight/mts-data-analysis-school/tree/main/mts-shad-fastapi-project)  
**Area:** backend for ML, API basics  
**Stack:** Python, FastAPI, SQLAlchemy, JWT, SQLite, pytest

A backend project built with FastAPI, including authentication, CRUD operations, SQLAlchemy, SQLite and tests.  
It is not an ML project directly, but it complements an MLE portfolio by showing an understanding of API layers and server-side development.

**Implemented:**

- REST API with FastAPI;
- database interaction with SQLAlchemy;
- JWT authentication;
- CRUD operations;
- tests with pytest.

**Why it matters:**  
For MLE roles, it is important not only to train models, but also to understand how to expose functionality through APIs and integrate it into services.

---

## Additional Projects

| Project | Path | Short Description |
|---|---|---|
| Rent Price Regression | `mts-data-analysis-school/ml2` / `portfolio` | Rental price prediction with CatBoost, Optuna and SHAP. |
| Scrapy Film Parser | `mts-data-analysis-school/wiki-films-scrapy-project` | Film data parser with CSV export. |
| Route Planner | `case-hack-projects/route-project` | Route planning project using graph algorithms. |
