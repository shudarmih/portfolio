# Определение возраста покупателей

[ipynb](https://github.com/shudarmih/portfolio/blob/main/02%20determining%20the%20buyer's%20age%20from%20a%20photo/determining%20the%20buyer's%20age%20from%20a%20photo.ipynb)

## Описание проекта
Требуется подготовить прототип модели машинного обучения, которая должна предсказать возраст покупателя в прикассовой зоне магазина. Модель поможет контролировать допросовестность кассиров при продаже алкоголя и предлагать товары, которые могут заинтересовать покупателя.

## Навыки и инструменты
numpy 
pandas 
matplotlib.pyplot 
seaborn
PIL.Image
tensorflow.keras.models.Sequential
tensorflow.keras.layers.Dense
tensorflow.keras.layers.GlobalAveragePooling2D
tensorflow.keras.applications.resnet.ResNet50
tensorflow.keras.preprocessing.image.ImageDataGenerator 

## Общий вывод
Для предсказания возраста была обучена модель, созданная на основе ResNet50. Метрика MAE на тестовом наборе данных = 7.1515
