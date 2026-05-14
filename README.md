# Портфолио проектов — Data Science / ML Engineering

## Основные проекты

---

## 1. CV Analyzer — анализ ИИ-компетенций по резюме и GitHub

**Репозиторий:** `cv-analyzer-gazprom-neft`  
**Направление:** NLP, ML-сервис, HRTech

Сервис для анализа резюме и GitHub-профиля кандидата по матрице ИИ-компетенций. Решение оценивает соответствие кандидата выбранной роли, показывает сильные и слабые стороны профиля и формирует рекомендации.

В проекте были реализованы два пользовательских сценария: интерфейс кандидата и HR-интерфейс для просмотра заявок.

**Моя роль:**

- дообучение модели для анализа компетенций;
- участие в разработке Streamlit-приложения;
- докеризация сервиса;
- настройка сервера;
- участие в проработке логики продукта.

**Стек:** Python, Streamlit, Transformers, XLM-RoBERTa, PostgreSQL, Docker, GitHub API

**Результат:** 1-е место в ML кейс-чемпионате «ProЦифру».

---

## 2. RAG-сервис для интеллектуального поиска по корпоративному Excel-реестру

**Тип проекта:** стажировка / коммерческий проект  
**Направление:** RAG, поиск, обработка табличных данных, LLM

Прототип сервиса для поиска проектной информации в корпоративном Excel-реестре. Данные были представлены не как обычные документы, а как набор связанных таблиц: проекты, сценарии, НИОКР, поставщики, материалы бенчмаркинга и связи между сущностями.

Сервис преобразует строки Excel в структурированные документы, строит поисковый индекс и позволяет искать не только по точным словам, но и по смысловой близости. Ответ формируется с опорой на найденные источники, чтобы пользователь мог проверить результат.

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

## 3. Real-Time Fraud Detection System

**Путь:** `mts-data-analysis-school/ml-ops-2`  
**Направление:** ML-сервис, потоковая обработка, MLOps

Проект потоковой системы для определения мошеннических транзакций. В отличие от обычного ноутбука с моделью, здесь был собран сценарий, приближенный к сервисной архитектуре: события поступают в поток, модель рассчитывает риск, результат сохраняется и отображается в интерфейсе.

**Что было реализовано:**

- генерация событий транзакций;
- передача данных через Kafka;
- ML-сервис для скоринга транзакций;
- сохранение результатов в PostgreSQL;
- Streamlit-интерфейс для мониторинга;
- контейнеризация компонентов.

**Стек:** Python, Kafka, PostgreSQL, CatBoost, Streamlit, Docker

---

## 4. Multi-Agent Interview Coach

**Репозиторий:** `ITMO_megaschool_case_3`  
**Направление:** LLM, агенты, симуляция интервью

Приложение для проведения тренировочного технического собеседования. Система анализирует профиль кандидата, задаёт вопросы, проверяет ответы и собирает итоговый отчёт с обратной связью.

Проект построен как набор агентов с разными ролями: один отвечает за сбор исходной информации, другой проводит интервью, отдельный агент проверяет ответы, а финальный агент формирует отчёт.

**Что было реализовано:**

- сценарий mock interview;
- агентная структура;
- управление состоянием диалога;
- проверка ответов через отдельный модуль;
- отчёт по итогам интервью;
- Streamlit-интерфейс.

**Стек:** Python, LangGraph, Streamlit, GigaChat API, Pydantic

---

## 5. Fraud Detection — классификация мошеннических транзакций

**Путь:** `mts-data-analysis-school/ml1`  
**Направление:** классический ML, антифрод, классификация

Проект по выявлению мошеннических транзакций. Задача решалась как бинарная классификация: по признакам операции нужно определить, является ли транзакция подозрительной.

В проекте были обработаны транзакционные данные, подготовлены признаки, обучена модель и проведена оценка качества. Отдельное внимание уделялось подбору гиперпараметров и интерпретации результата.

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

## 6. Rent Price Prediction — прогнозирование стоимости аренды

**Путь:** `mts-data-analysis-school/ml2`  
**Направление:** регрессия, оценка стоимости, классический ML

Проект по прогнозированию стоимости аренды жилья. Задача заключалась в том, чтобы по характеристикам объекта оценить ожидаемую цену аренды.

В проекте были обработаны пропуски и категориальные признаки, добавлены новые признаки, обучена регрессионная модель и проведена интерпретация факторов, влияющих на итоговую цену.

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

## 7. NLP Salary Prediction

**Путь:** `mts-data-analysis-school/nn1`  
**Направление:** NLP, регрессия по текстовым данным

Проект по прогнозированию зарплаты на основе описания вакансии. Основная часть задачи связана с обработкой текста: нужно извлечь полезную информацию из описания и использовать её для оценки зарплатного диапазона.

**Что было сделано:**

- обработка текстов вакансий;
- подготовка текстовых признаков;
- сравнение классических и нейросетевых подходов;
- обучение моделей регрессии;
- оценка качества предсказаний.

**Стек:** Python, PyTorch, Transformers, TF-IDF, scikit-learn

---

## 8. Stacking Models with Uncertainty Estimation

**Путь:** `mts-data-analysis-school/ml3` / `portfolio`  
**Направление:** ансамбли, регрессия, оценка неопределённости

Проект по построению ансамбля регрессионных моделей. Использовались несколько моделей разного типа, а затем их предсказания объединялись через мета-модель.

Дополнительно рассматривалась неопределённость предсказаний: насколько можно доверять результату модели и как ошибка связана с уровнем уверенности.

**Что было сделано:**

- пайплайн предобработки данных;
- обучение CatBoost, LightGBM, XGBoost, RandomForest и Ridge;
- стекинг моделей;
- подбор гиперпараметров;
- оценка неопределённости;
- анализ ошибок и доверия к предсказаниям.

**Стек:** Python, scikit-learn, CatBoost, LightGBM, XGBoost, Optuna, SHAP

---

## 9. Image Preference Prediction

**Путь:** `mts-data-analysis-school/nn2`  
**Направление:** Computer Vision, эмбеддинги, классификация

Проект по определению более предпочтительного изображения из пары. Вместо обучения модели с нуля использовались эмбеддинги предобученной модели CLIP, а поверх них обучался классификатор.

**Что было сделано:**

- получение эмбеддингов изображений;
- работа с предобученной CLIP-моделью;
- подготовка признаков для пар изображений;
- обучение классификатора;
- оценка качества модели.

**Стек:** Python, PyTorch, CLIP, CatBoost

---

## Дополнительные проекты

### RAG по PDF-документу

**Путь:** `mts-data-analysis-school/nn3`

Учебный RAG-пайплайн по PDF-документу. Реализованы разбиение текста, построение индекса, поиск релевантных фрагментов и генерация ответа по найденному контексту.

**Стек:** Python, LangChain, Chroma, BM25Retriever, EnsembleRetriever, multilingual-e5, Ollama

---

### FastAPI Seller & Books Project

**Путь:** `mts-data-analysis-school/mts-shad-fastapi-project`

Backend-проект на FastAPI с авторизацией, CRUD-операциями, SQLAlchemy, SQLite и тестами. В портфолио он вынесен в дополнительные проекты: он показывает базовое понимание API и серверной части, но не является ключевым ML-проектом.

**Стек:** Python, FastAPI, SQLAlchemy, JWT, SQLite, pytest

---

# Project Portfolio — Data Science / ML Engineering

## Main projects

---

## 1. CV Analyzer — AI Competency Assessment from CV and GitHub

**Repository:** `cv-analyzer-gazprom-neft`  
**Area:** NLP, ML service, HRTech

A service for analyzing a candidate’s CV and GitHub profile against an AI competency matrix. The application estimates how well the candidate matches a selected role, highlights strengths and weaknesses, and generates recommendations.

The project included two main user scenarios: a candidate interface and an HR interface for reviewing applications.

**My role:**

- fine-tuning a model for competency analysis;
- contributing to the Streamlit application;
- Dockerizing the service;
- setting up the server;
- working on the product logic.

**Stack:** Python, Streamlit, Transformers, XLM-RoBERTa, PostgreSQL, Docker, GitHub API

**Result:** 1st place in the “ProЦифру” ML case championship.

---

## 2. RAG Search Service for a Corporate Excel Registry

**Project type:** internship / commercial project  
**Area:** RAG, search, tabular data processing, LLM

A prototype of an intelligent search service for a corporate Excel-based project registry. The source data was not a set of plain documents, but a group of connected tables: projects, scenarios, R&D items, suppliers, benchmarking materials and relations between entities.

The service converts Excel rows into structured searchable documents, builds a search index and supports both exact keyword search and semantic search. The answer is generated using retrieved sources, so the user can verify the result.

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

## 3. Real-Time Fraud Detection System

**Path:** `mts-data-analysis-school/ml-ops-2`  
**Area:** ML service, streaming data, MLOps

A streaming system for detecting fraudulent transactions. Unlike a regular notebook-based model, this project is closer to a service architecture: events are sent to a stream, the model scores transaction risk, the result is stored and displayed in an interface.

**Implemented:**

- transaction event generation;
- data transfer through Kafka;
- ML service for transaction scoring;
- result storage in PostgreSQL;
- Streamlit monitoring interface;
- containerized components.

**Stack:** Python, Kafka, PostgreSQL, CatBoost, Streamlit, Docker

---

## 4. Multi-Agent Interview Coach

**Repository:** `ITMO_megaschool_case_3`  
**Area:** LLM, agents, interview simulation

An application for technical mock interviews. The system analyzes a candidate profile, asks interview questions, checks answers and produces a final feedback report.

The project is built as a group of agents with different roles: one collects initial information, another conducts the interview, a separate agent checks the answers, and the final agent prepares the report.

**Implemented:**

- mock interview scenario;
- agent-based structure;
- dialogue state management;
- answer checking module;
- final interview report;
- Streamlit interface.

**Stack:** Python, LangGraph, Streamlit, GigaChat API, Pydantic

---

## 5. Fraud Detection — Transaction Classification

**Path:** `mts-data-analysis-school/ml1`  
**Area:** classical ML, fraud detection, classification

A project for detecting fraudulent transactions. The task was formulated as binary classification: based on transaction features, the model predicts whether a transaction is suspicious.

The project included transaction data preprocessing, feature preparation, model training and quality evaluation. Hyperparameter tuning and result interpretation were also included.

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

## 6. Rent Price Prediction

**Path:** `mts-data-analysis-school/ml2`  
**Area:** regression, price estimation, classical ML

A project for predicting rental housing prices. The goal was to estimate the expected rental price based on property characteristics.

The project included missing value handling, categorical feature processing, feature engineering, model training and interpretation of price-driving factors.

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

## 7. NLP Salary Prediction

**Path:** `mts-data-analysis-school/nn1`  
**Area:** NLP, text-based regression

A project for predicting salary from vacancy descriptions. The main part of the task was text processing: extracting useful information from job descriptions and using it to estimate salary.

**Implemented:**

- vacancy text processing;
- text feature preparation;
- comparison of classical and neural approaches;
- regression model training;
- prediction quality evaluation.

**Stack:** Python, PyTorch, Transformers, TF-IDF, scikit-learn

---

## 8. Stacking Models with Uncertainty Estimation

**Path:** `mts-data-analysis-school/ml3` / `portfolio`  
**Area:** ensembles, regression, uncertainty estimation

A project focused on building a regression ensemble. Several different models were trained, and their predictions were combined using a meta-model.

The project also explored prediction uncertainty: how much the model’s output can be trusted and how prediction error relates to confidence.

**Implemented:**

- preprocessing pipeline;
- training CatBoost, LightGBM, XGBoost, RandomForest and Ridge;
- model stacking;
- hyperparameter tuning;
- uncertainty estimation;
- error and confidence analysis.

**Stack:** Python, scikit-learn, CatBoost, LightGBM, XGBoost, Optuna, SHAP

---

## 9. Image Preference Prediction

**Path:** `mts-data-analysis-school/nn2`  
**Area:** Computer Vision, embeddings, classification

A project for predicting the preferred image from a pair. Instead of training an image model from scratch, the project uses embeddings from a pretrained CLIP model and trains a classifier on top of them.

**Implemented:**

- image embedding extraction;
- use of a pretrained CLIP model;
- feature preparation for image pairs;
- classifier training;
- model quality evaluation.

**Stack:** Python, PyTorch, CLIP, CatBoost

---

## Additional projects

### RAG over a PDF Document

**Path:** `mts-data-analysis-school/nn3`

An educational RAG pipeline over a PDF document. The project includes text splitting, index creation, relevant fragment retrieval and answer generation based on retrieved context.

**Stack:** Python, LangChain, Chroma, BM25Retriever, EnsembleRetriever, multilingual-e5, Ollama

---

### FastAPI Seller & Books Project

**Path:** `mts-data-analysis-school/mts-shad-fastapi-project`

A backend project built with FastAPI, authentication, CRUD operations, SQLAlchemy, SQLite and tests. It is listed as an additional project: it shows basic API and backend understanding, but it is not one of the main ML projects.

**Stack:** Python, FastAPI, SQLAlchemy, JWT, SQLite, pytest
