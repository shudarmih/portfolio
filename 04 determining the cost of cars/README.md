# Определение стоимости автомобилей

[ipynb](https://github.com/shudarmih/portfolio/blob/main/04%20determining%20the%20cost%20of%20cars/determining%20the%20cost%20of%20cars.ipynb)

## Описание проекта
Необходимо разработать модель для прогнозирования цены автомобиля. Модель будет использоваться в приложении, где потенциальныме клиенты смогут быстро узнать стоимость своего автомобиля

## Навыки и инструменты
numpy 
pandas 
matplotlib.pyplot 
seaborn
phik
sklearn

## Общий вывод
Выбрана модель со следующими параметрами: DecisionTreeRegressor(max_depth=15, min_samples_leaf=4, min_samples_split=9) с использованием StandardScaler() 
Значения метрики RMSE:

    2081,0 для тренировочных данных
    2050,8 для тестовых данных

Время обучения модели: 3.4 минуты.

Время предсказания: 235 мсек



