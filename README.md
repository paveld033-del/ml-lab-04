# Lab 04 — Регуляризация и градиентный спуск

Практические задания по регуляризации линейных моделей и методу градиентного спуска:
полиномиальные признаки и переобучение на зашумлённой синусоиде, регрессии Ridge и Lasso,
подготовка данных о ценах на жильё в Эймсе (one-hot кодирование, логарифмирование
асимметричных признаков), подбор гиперпараметров кросс-валидацией (`RidgeCV`, `LassoCV`,
`ElasticNetCV`) и стохастический градиентный спуск (`SGDRegressor`) с масштабированием
и без него, с ускорением через Intel® Extension for Scikit-learn.

Решение — в ноутбуке `04_Regularization_and_Gradient_Descent_Exercises.ipynb`,
данные — в `data/X_Y_Sinusoid_Data.csv` и `data/Ames_Housing_Sales.csv`.

## Запуск

```bash
uv sync
uv run jupyter lab
```

JupyterLab ставится в то же окружение `.venv`, что и scikit-learn-intelex: при запуске через
`uv run --with jupyter` ядро не находит DLL расширения Intel и падает с `ImportError`.
