# Оптимизация работы с персоналом: минимизация потерь и избегание оттока сотрудников.

[ipynb](https://github.com/shudarmih/portfolio/blob/main/07%20Optimization%20of%20work%20with%20personnel/Optimization%20of%20work%20with%20personnel.ipynb)

## Описание проекта
Требуется разработать следующие модели:
1. Модель для предсказания уровеня удовлетворенности сотрудников.
2. Модель для предсказания увольненеия сотрудника

## Навыки и инструменты
numpy 
pandas 
matplotlib
seaborn
phik
sklearn
shap

## Общий вывод
 - Задача 1: предсказание удовлетворенности сотриднков
 - Задача 2: предсказание увольненеия сотрудников
Для решения **Задачи 1 была подобрана модель: DecisionTreeRegressor()** с параметрами:
- max_depth=15
- min_samples_leaf=4
- min_samples_split=9 
    
Лучшая стандартизация для числовых переменных: MinMaxScaler()

Для оценки эффективности модели исползовалась метрика SMAPE.

Сравнение метрик SMAPE:

    14.899 - для тренировочных данных
    13.504 - для тестовых данных

Для решения **Задачи 2 была подобрана модель: DecisionTreeClassifier()** с параметрами:
 - max_depth=5
 - min_samples_leaf=6
 - min_samples_split=3
Лучшая стандартизация для числовых переменных: StandardScaler()

Для оценки эффективности модели исползовалась метрика ROC-AUC

Сравнение метрик SMAPE:
 - 0.903 для тренировочных данных
 - 0.920 - для тестовых данных

**Рекомендации для заказчика (на основе анализа значимости признаков)**
 - salary - зарплата является одинм из важных признаков для того, чтообы сотрудник был удовлетворен. Необходимо рассмотреть дополнительную материальную мотивацию для сотрудников с низкими зарплатами.
 - level - наиболее удовлетворены сотрудники уровня middle. Сотрудники уровней junior и sinior удовлетворены меньше. Необходимо провести дополнительные исследования среди сотрудников соответсвующих уровней.
 - workload - чем выше загрузка, тем чаще люди увольняются. Возможно, стоит пересмотреть способы распределения нагрузки по сотрудникам.
 - dept (sales) - в отделе продаж наибольшая текучка. Стоит провести дополнительное исследование сотрудников отдела, т.к. из имеющихся параметров ни один не влияет на повышение увольнений из отдела продаж.
