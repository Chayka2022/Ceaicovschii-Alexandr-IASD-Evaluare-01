# Evaluare 01: Învățarea supervizată

Решение аттестации №1 по дисциплине IASD на тему «Обучение с учителем» (supervised learning).

Выполнил: Alexandr Ceaicovschii

## Содержимое репозитория

| Файл | Описание |
|---|---|
| `Ceaicovschii_Alexandr_Evaluare_1.ipynb` | Решение в формате Jupyter Notebook: код, результаты вычислений и графики |
| `Ceaicovschii_Alexandr_Evaluare_1.pdf` | PDF-версия решения для просмотра без Jupyter |
| `archive/train.csv`, `archive/test.csv` | Исходные данные |

## Набор данных

[Human Activity Recognition Using Smartphones](https://www.kaggle.com/datasets/uciml/human-activity-recognition-with-smartphones) (UCI HAR). Данные записаны с акселерометра и гироскопа смартфона, закреплённого на поясе у 30 участников. Набор содержит 10 299 наблюдений и 561 числовой признак. Целевая переменная `Activity` принимает шесть значений: WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING.

## Содержание работы

1. Загрузка данных, проверка размерности, типов и пропущенных значений.
2. Визуализация: диаграмма рассеяния и тепловая карта корреляций.
3. Линейная регрессия, оценка по метрикам MAE, MSE и RMSE.
4. Метод k ближайших соседей (KNN), перекрёстная проверка и подбор k.
5. Линейная регрессия, логистическая регрессия для бинарной классификации, SVM.
6. Матрица ошибок для логистической регрессии.
7. Реализация градиентного спуска вручную.
8. Случайный лес, AdaBoost и бэггинг.
9. Стекинг: Random Forest, SVM и логистическая регрессия, мета-модель — логистическая регрессия.

## Основные результаты

Точность (accuracy) классификации вида активности на тестовой выборке:

| Модель | Accuracy |
|---|---|
| Стекинг | 0.989 |
| AdaBoost | 0.988 |
| Логистическая регрессия | 0.986 |
| Random Forest | 0.981 |
| SVM | 0.976 |
| Бэггинг | 0.965 |
| KNN (k = 5) | 0.965 |

## Запуск

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook Ceaicovschii_Alexandr_Evaluare_1.ipynb
```
