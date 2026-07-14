<div align="center">

# 📈 Retail Turnover Forecasting

Machine Learning solutions for forecasting monthly retail turnover (RTO) of **Pyaterochka** stores.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![License](https://img.shields.io/badge/License-MIT-green)

English | [Русский](#-русский)

</div>

---

# 🇬🇧 English

## Overview

This repository contains two independent machine learning solutions developed for the **X5 Group "Gradient of Growth" Hackathon**.

The objective is to forecast the monthly **Retail Turnover (RTO)** of Pyaterochka stores one month ahead using historical sales, store characteristics, customer behavior, and local infrastructure.

---

## Pipeline

```text
Raw data
    │
    ▼
Data validation
    │
    ▼
Exploratory Data Analysis
    │
    ▼
Feature Engineering
    │
    ▼
Time-based validation
    │
    ▼
Model training
    │
    ▼
Post-processing
    │
    ▼
Submission
```

---

## Repository Structure

```text
Retail-Turnover-Forecasting/
│
├── stage1_train/
│   ├── random_forest.ipynb
│   ├── README.md
│   └── requirements.txt
│
├── stage2_train2/
│   ├── solution.ipynb
│   ├── README.md
│   ├── requirements.txt
│   └── analysis/
│       ├── target_distribution.png
│       ├── seasonality_by_month.png
│       ├── spearman_correlation_matrix.png
│       ├── full_correlation_matrix.png
│       └── yoy_growth_janfeb.png
│
├── LICENSE
├── README.md
└── .gitignore
```

---

## Results

| Stage | Model | Holdout / Final Result |
|------|------|------------------------:|
| Stage 1 | Random Forest | **MAPE = 2.78%** |
| Stage 2 | CatBoost + Feature Engineering + Adaptive Clipping | **MAPE ≈ 7.67% (82.69 points)** |

---

## Technologies

- Python
- Pandas
- NumPy
- CatBoost
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Reproducibility

Each stage contains its own notebook, documentation, and dependency list, allowing every experiment to be reproduced independently.

---

# 🇷🇺 Русский

## О проекте

В репозитории представлены два независимых решения задачи прогнозирования месячного **розничного товарооборота (РТО)** магазинов сети **«Пятёрочка»**, разработанные в рамках хакатона **X5 Group «Градиент роста»**.

Цель проекта — спрогнозировать РТО каждого магазина на следующий месяц на основе истории продаж, характеристик магазина, инфраструктуры и временных закономерностей.

---

## Пайплайн

```text
Исходные данные
      │
      ▼
Проверка качества данных
      │
      ▼
Разведочный анализ (EDA)
      │
      ▼
Feature Engineering
      │
      ▼
Time-based валидация
      │
      ▼
Обучение модели
      │
      ▼
Постобработка прогнозов
      │
      ▼
Формирование решения
```

---

## Структура репозитория

```text
Retail-Turnover-Forecasting/
│
├── stage1_train/
├── stage2_train2/
├── LICENSE
├── README.md
└── .gitignore
```

---

## Результаты

| Этап | Модель | Результат |
|------|---------|----------:|
| Этап 1 | Random Forest | **MAPE = 2.78%** |
| Этап 2 | CatBoost + Feature Engineering + Adaptive Clipping | **MAPE ≈ 7.67% (82.69 балла)** |

---

## Используемые технологии

- Python
- Pandas
- NumPy
- CatBoost
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Воспроизводимость

Каждый этап содержит:

- ноутбук;
- README;
- requirements.txt.

Благодаря этому каждое решение можно воспроизвести независимо.

---

## Лицензия

MIT License.