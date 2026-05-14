# Портфолио проектов — Data Science / ML Engineering

## Основные проекты

---

## 1. [CV Analyzer — анализ ИИ-компетенций по резюме и GitHub](https://github.com/KsyLight/cv-analyzer-gazprom-neft)

**Репозиторий:** [`cv-analyzer-gazprom-neft`](https://github.com/KsyLight/cv-analyzer-gazprom-neft)  
**Направление:** NLP, ML-сервис, HRTech

Сервис для анализа резюме и GitHub-профиля кандидата по матрице ИИ-компетенций. Решение оценивает соответствие кандидата выбранной роли, выделяет сильные и слабые стороны профиля и формирует рекомендации.

В проекте были реализованы интерфейс кандидата и HR-интерфейс для просмотра заявок.

**Моя роль:**

- дообучение модели для анализа компетенций;
- участие в разработке Streamlit-приложения;
- докеризация сервиса;
- настройка сервера;
- участие в проработке логики продукта.

**Стек:** Python, Streamlit, Transformers, XLM-RoBERTa, PostgreSQL, Docker, GitHub API

**Результат:** 1-е место в кейс-чемпионате «ProЦифру».

---

## 2. RAG-сервис для интеллектуального поиска по корпоративному Excel-реестру

**Ссылка:** закрытый / непубличный проект  
**Тип проекта:** стажировка / коммерческий проект  
**Направление:** RAG, поиск, обработка табличных данных, LLM

Прототип сервиса для поиска проектной информации в корпоративном Excel-реестре. Данные представлены как набор связанных таблиц: проекты, сценарии, НИОКР, поставщики, материалы бенчмаркинга и связи между сущностями.

Сервис преобразует строки Excel в структурированные документы, строит поисковый индекс и позволяет искать не только по точному совпадению, но и по смысловой близости. Ответ формируется с опорой на найденные источники.

**Что было реализовано:**

- чтение и обработка Excel-реестра;
- преобразование строк таблиц в документы для поиска;
- учёт метаданных, идентификаторов и связей между объектами;
- гибридный поиск: BM25 + векторный поиск;
- повторное ранжирование найденных записей;
- генерация ответа с привязкой к источникам;
- интерфейс для поиска и просмотра найденных материалов.

**Стек:** Python, Pandas, OpenPyXL, LangChain, ChromaDB, BM25, эмбеддинги, Streamlit, LLM API

---

## 3. [Потоковая система антифрода](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml-ops-2)

**Путь:** [`mts-data-analysis-school/ml-ops-2`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml-ops-2)  
**Направление:** ML-сервис, потоковая обработка, MLOps

Проект потоковой системы для определения мошеннических транзакций. События транзакций поступают в поток, модель рассчитывает риск, результат сохраняется в базу данных и отображается в интерфейсе мониторинга.

**Что было реализовано:**

- генерация событий транзакций;
- передача данных через Kafka;
- ML-сервис для скоринга транзакций;
- сохранение результатов в PostgreSQL;
- Streamlit-интерфейс для мониторинга;
- контейнеризация компонентов.

**Стек:** Python, Kafka, PostgreSQL, CatBoost, Streamlit, Docker

---

## 4. [Multi-Agent Interview Coach](https://github.com/KsyLight/ITMO_megaschool_case_3)

**Репозиторий:** [`ITMO_megaschool_case_3`](https://github.com/KsyLight/ITMO_megaschool_case_3)  
**Направление:** LLM, агенты, симуляция интервью

Приложение для проведения тренировочного технического собеседования. Система анализирует профиль кандидата, задаёт вопросы, проверяет ответы и формирует итоговый отчёт с обратной связью.

Проект построен как набор агентов с разными ролями: сбор исходной информации, проведение интервью, проверка ответов и подготовка отчёта.

**Что было реализовано:**

- сценарий тренировочного интервью;
- агентная структура;
- управление состоянием диалога;
- проверка ответов через отдельный модуль;
- отчёт по итогам интервью;
- Streamlit-интерфейс.

**Стек:** Python, LangGraph, Streamlit, GigaChat API, Pydantic

---

## 5. [Fraud Detection — классификация мошеннических транзакций](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml1)

**Путь:** [`mts-data-analysis-school/ml1`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml1)  
**Направление:** классический ML, антифрод, классификация

Проект по выявлению мошеннических транзакций. Задача решалась как бинарная классификация: по признакам операции нужно определить, является ли транзакция подозрительной.

**Что было сделано:**

- предобработка транзакционных данных;
- создание признаков;
- обучение CatBoostClassifier;
- подбор гиперпараметров через Optuna;
- оценка качества по F1-score и logloss;
- анализ важности признаков.

**Стек:** Python, Pandas, CatBoost, scikit-learn, Optuna, SHAP

**Результат:** 1-е место в Kaggle-соревновании ШАД МТС.

---

## 6. [Rent Price Prediction — прогнозирование стоимости аренды](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml2)

**Путь:** [`mts-data-analysis-school/ml2`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml2)  
**Направление:** регрессия, оценка стоимости, классический ML

Проект по прогнозированию стоимости аренды жилья. По характеристикам объекта модель оценивает ожидаемую цену аренды.

**Что было сделано:**

- очистка и подготовка данных;
- обработка категориальных и числовых признаков;
- логарифмирование целевой переменной;
- обучение CatBoostRegressor;
- подбор гиперпараметров через Optuna;
- оценка качества по RMSE, MSE и R²;
- анализ признаков через SHAP.

**Стек:** Python, Pandas, CatBoost, scikit-learn, Optuna, SHAP, Statsmodels

---

## 7. [NLP Salary Prediction](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn1)

**Путь:** [`mts-data-analysis-school/nn1`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn1)  
**Направление:** NLP, регрессия по текстовым данным

Проект по прогнозированию зарплаты на основе описания вакансии. Основной фокус — обработка текстов вакансий и использование текстовых признаков для оценки зарплатного диапазона.

**Что было сделано:**

- обработка текстов вакансий;
- подготовка текстовых признаков;
- сравнение классических и нейросетевых подходов;
- обучение моделей регрессии;
- оценка качества предсказаний.

**Стек:** Python, PyTorch, Transformers, TF-IDF, scikit-learn

---

## 8. [Stacking Models with Uncertainty Estimation](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml3)

**Путь:** [`mts-data-analysis-school/ml3`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml3) / [`portfolio`](https://github.com/KsyLight/portfolio)  
**Направление:** ансамбли, регрессия, оценка неопределённости

Проект по построению ансамбля регрессионных моделей. Предсказания нескольких моделей объединяются через мета-модель, дополнительно оценивается неопределённость результата.

**Что было сделано:**

- пайплайн предобработки данных;
- обучение CatBoost, LightGBM, XGBoost, RandomForest и Ridge;
- стекинг моделей;
- подбор гиперпараметров;
- оценка неопределённости;
- анализ ошибок и доверия к предсказаниям.

**Стек:** Python, scikit-learn, CatBoost, LightGBM, XGBoost, Optuna, SHAP

---

## 9. [Определение предпочтительного изображения](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn2)

**Путь:** [`mts-data-analysis-school/nn2`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn2)  
**Направление:** Computer Vision, эмбеддинги, классификация

Проект по определению более предпочтительного изображения из пары. Используются эмбеддинги предобученной модели CLIP, поверх которых обучается классификатор.

**Что было сделано:**

- получение эмбеддингов изображений;
- работа с предобученной CLIP-моделью;
- подготовка признаков для пар изображений;
- обучение классификатора;
- оценка качества модели.

**Стек:** Python, PyTorch, CLIP, CatBoost

---

## Дополнительные проекты

### [RAG по PDF-документу](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn3)

**Путь:** [`mts-data-analysis-school/nn3`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn3)

Учебный RAG-пайплайн по PDF-документу. Реализованы разбиение текста, построение индекса, поиск релевантных фрагментов и генерация ответа по найденному контексту.

**Стек:** Python, LangChain, Chroma, BM25Retriever, EnsembleRetriever, multilingual-e5, Ollama

---

### [FastAPI Seller & Books Project](https://github.com/KsyLight/mts-data-analysis-school/tree/main/mts-shad-fastapi-project)

**Путь:** [`mts-data-analysis-school/mts-shad-fastapi-project`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/mts-shad-fastapi-project)

Backend-проект на FastAPI с авторизацией, CRUD-операциями, SQLAlchemy, SQLite и тестами. Вынесен в дополнительные проекты, так как показывает базовое понимание API, но не является ключевым ML-проектом.

**Стек:** Python, FastAPI, SQLAlchemy, JWT, SQLite, pytest

---

# Project Portfolio — Data Science / ML Engineering

## Main projects

---

## 1. [CV Analyzer — AI Competency Assessment from CV and GitHub](https://github.com/KsyLight/cv-analyzer-gazprom-neft)

**Repository:** [`cv-analyzer-gazprom-neft`](https://github.com/KsyLight/cv-analyzer-gazprom-neft)  
**Area:** NLP, ML service, HRTech

A service for analyzing a candidate’s CV and GitHub profile against an AI competency matrix. The application estimates role fit, highlights strengths and weaknesses, and generates recommendations.

The project included a candidate interface and an HR interface for reviewing applications.

**My role:**

- fine-tuning a model for competency analysis;
- contributing to the Streamlit application;
- Dockerizing the service;
- setting up the server;
- working on the product logic.

**Stack:** Python, Streamlit, Transformers, XLM-RoBERTa, PostgreSQL, Docker, GitHub API

**Result:** 1st place in the “ProЦифру” case competition.

---

## 2. RAG Search Service for a Corporate Excel Registry

**Link:** private / non-public project  
**Project type:** internship / commercial project  
**Area:** RAG, search, tabular data processing, LLM

A prototype of an intelligent search service for a corporate Excel-based project registry. The source data is a group of connected tables: projects, scenarios, R&D items, suppliers, benchmarking materials and relations between entities.

The service converts Excel rows into structured searchable documents, builds a search index and supports both exact keyword search and semantic search. The answer is generated using retrieved sources.

**Implemented:**

- Excel registry parsing;
- conversion of table rows into searchable documents;
- handling of metadata, identifiers and entity relations;
- hybrid retrieval: BM25 + vector search;
- reranking of retrieved records;
- answer generation with source references;
- interface for search and result inspection.

**Stack:** Python, Pandas, OpenPyXL, LangChain, ChromaDB, BM25, embeddings, Streamlit, LLM API

---

## 3. [Real-Time Fraud Detection System](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml-ops-2)

**Path:** [`mts-data-analysis-school/ml-ops-2`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml-ops-2)  
**Area:** ML service, streaming data, MLOps

A streaming system for detecting fraudulent transactions. Transaction events are sent to a stream, the model scores transaction risk, the result is stored in a database and displayed in a monitoring interface.

**Implemented:**

- transaction event generation;
- data transfer through Kafka;
- ML service for transaction scoring;
- result storage in PostgreSQL;
- Streamlit monitoring interface;
- containerized components.

**Stack:** Python, Kafka, PostgreSQL, CatBoost, Streamlit, Docker

---

## 4. [Multi-Agent Interview Coach](https://github.com/KsyLight/ITMO_megaschool_case_3)

**Repository:** [`ITMO_megaschool_case_3`](https://github.com/KsyLight/ITMO_megaschool_case_3)  
**Area:** LLM, agents, interview simulation

An application for technical interview practice. The system analyzes a candidate profile, asks questions, checks answers and produces a final feedback report.

The project is built as a group of agents with different roles: collecting initial information, conducting the interview, checking answers and preparing the report.

**Implemented:**

- interview practice scenario;
- agent-based structure;
- dialogue state management;
- answer checking module;
- final interview report;
- Streamlit interface.

**Stack:** Python, LangGraph, Streamlit, GigaChat API, Pydantic

---

## 5. [Fraud Detection — Transaction Classification](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml1)

**Path:** [`mts-data-analysis-school/ml1`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml1)  
**Area:** classical ML, fraud detection, classification

A project for detecting fraudulent transactions. The task was formulated as binary classification: based on transaction features, the model predicts whether a transaction is suspicious.

**Implemented:**

- transaction data preprocessing;
- feature engineering;
- CatBoostClassifier training;
- hyperparameter tuning with Optuna;
- evaluation using F1-score and logloss;
- feature importance analysis.

**Stack:** Python, Pandas, CatBoost, scikit-learn, Optuna, SHAP

**Result:** 1st place in the MTS Data Analysis School Kaggle competition.

---

## 6. [Rent Price Prediction](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml2)

**Path:** [`mts-data-analysis-school/ml2`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml2)  
**Area:** regression, price estimation, classical ML

A project for predicting rental housing prices. The model estimates the expected rental price based on property characteristics.

**Implemented:**

- data cleaning and preparation;
- processing of categorical and numerical features;
- target variable log transformation;
- CatBoostRegressor training;
- hyperparameter tuning with Optuna;
- evaluation using RMSE, MSE and R²;
- feature analysis with SHAP.

**Stack:** Python, Pandas, CatBoost, scikit-learn, Optuna, SHAP, Statsmodels

---

## 7. [NLP Salary Prediction](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn1)

**Path:** [`mts-data-analysis-school/nn1`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn1)  
**Area:** NLP, text-based regression

A project for predicting salary from vacancy descriptions. The main focus is text processing and using text features to estimate salary.

**Implemented:**

- vacancy text processing;
- text feature preparation;
- comparison of classical and neural approaches;
- regression model training;
- prediction quality evaluation.

**Stack:** Python, PyTorch, Transformers, TF-IDF, scikit-learn

---

## 8. [Stacking Models with Uncertainty Estimation](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml3)

**Path:** [`mts-data-analysis-school/ml3`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/ml3) / [`portfolio`](https://github.com/KsyLight/portfolio)  
**Area:** ensembles, regression, uncertainty estimation

A regression ensemble project. Predictions from several models are combined using a meta-model, with an additional focus on prediction uncertainty.

**Implemented:**

- preprocessing pipeline;
- training CatBoost, LightGBM, XGBoost, RandomForest and Ridge;
- model stacking;
- hyperparameter tuning;
- uncertainty estimation;
- error and confidence analysis.

**Stack:** Python, scikit-learn, CatBoost, LightGBM, XGBoost, Optuna, SHAP

---

## 9. [Image Preference Prediction](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn2)

**Path:** [`mts-data-analysis-school/nn2`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn2)  
**Area:** Computer Vision, embeddings, classification

A project for predicting the preferred image from a pair. The project uses embeddings from a pretrained CLIP model and trains a classifier on top of them.

**Implemented:**

- image embedding extraction;
- use of a pretrained CLIP model;
- feature preparation for image pairs;
- classifier training;
- model quality evaluation.

**Stack:** Python, PyTorch, CLIP, CatBoost

---

## Additional projects

### [RAG over a PDF Document](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn3)

**Path:** [`mts-data-analysis-school/nn3`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/nn3)

An educational RAG pipeline over a PDF document. The project includes text splitting, index creation, relevant fragment retrieval and answer generation based on retrieved context.

**Stack:** Python, LangChain, Chroma, BM25Retriever, EnsembleRetriever, multilingual-e5, Ollama

---

### [FastAPI Seller & Books Project](https://github.com/KsyLight/mts-data-analysis-school/tree/main/mts-shad-fastapi-project)

**Path:** [`mts-data-analysis-school/mts-shad-fastapi-project`](https://github.com/KsyLight/mts-data-analysis-school/tree/main/mts-shad-fastapi-project)

A backend project built with FastAPI, authentication, CRUD operations, SQLAlchemy, SQLite and tests. It is listed as an additional project because it shows basic API knowledge but is not one of the main ML projects.

**Stack:** Python, FastAPI, SQLAlchemy, JWT, SQLite, pytest
