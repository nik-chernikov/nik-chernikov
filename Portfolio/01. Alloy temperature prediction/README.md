# Alloy temperature prediction

### Tools used

PyTorch, LightGBM, SQLAlchemy, pandas, Matplotlib, scikit-learn

### Key features

Machine learning, gradient boosting, Multilayer Perceptron

### Task description

To optimize production costs, the Steel Bird metallurgical plant decided to reduce electricity consumption during the steel processing stage. To achieve this, the plant must control the alloy temperature. Your task is to build a model that will predict it. The customer wants to use the developed model to simulate the technological process. Study it before generating new features.

The target feature is the final temperature of the batch.

### General conclusion

We conducted a research analysis of the data, generated new features, combined the data, and investigated the correlation in the data. 

After that, we trained several models: RandomForestRegressor, SGD, LightGBM, and the Multilayer Perceptron neural network. 

The RandomForestRegressor model performed best. After testing the model on a test sample, we obtained a target MAE value of 6.5492. This is lower than the required MAE value of 6.8.

Finally, we conducted a study of the importance of features in the model and highlighted that the features StartTemperature, HeatTime, Wire 1, and Bulk 6 have a significant impact on the model's predictions.


---
# Предсказание температуры сплава

### Использованные инструменты

PyTorch, LightGBM, SQLAlchemy, pandas, Matplotlib, scikit-learn 

### Ключевые особенности

Машинное обучение, градиентный бустинг, Multilayer Perceptron

### Описание задачи

Чтобы оптимизировать производственные расходы, металлургический комбинат «Стальная птица» решил уменьшить потребление электроэнергии на этапе обработки стали. Для этого комбинату нужно контролировать температуру сплава. Ваша задача — построить модель, которая будет её предсказывать. Заказчик хочет использовать разработанную модель для имитации технологического процесса. Изучите его, прежде чем генерировать новые признаки.

Целевой признак — последняя температура партии.

### Общий вывод

Мы провели исследовательский анализ данных, сгенерировали новые признаки, объединили данные и исследовали корреляцию в данных. 

После этого мы обучили несколько моделей: RandomForestRegressor, SGD, LightGBM, и нейросеть Multilayer Perceptron. 

Лучше всего себя показала модель RandomForestRegressor. Протестировав модель на тестовой выборке мы получили целевое значение MAE, равное 6.5492. Это ниже требуемого значения в MAE 6.8

В конце мы провели исследование важности признаков в модели и можем выделить, что признаки StartTemperature, HeatTime, Wire 1, Bulk 6 оказывают существенное влияние на предсказания модели.