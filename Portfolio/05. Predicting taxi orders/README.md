# Predicting taxi orders for the next hour

### Tools used

statsmodels, LightGBM, pandas, scikit-learn, Matplotlib

### Key features

Time series, regression

### Task description

The company "Chyotenkoe taxi" collected historical data on taxi orders at airports. In order to attract more drivers during peak load periods, it is necessary to predict the number of taxi orders for the next hour. Build a model for such a prediction.

The value of the _RMSE_ metric on the test sample should be no more than 48.

You need to:

1. Load the data and resample it by one hour.
2. Analyze the data.
3. Train different models with different hyperparameters. Make a test sample of 10% of the original data.
4. Check the data on the test sample and conclude.

### General conclusion

We had a time series containing almost 26,500 records. A trend towards an increase in the number of orders over time is noticeable.

We analyzed the data and prepared a detailed conclusion.

To achieve the optimal result, we added additional features to our dataset: 168th lag and 24-hour moving average.

We trained several models using cross-validation and chose the best one. It turned out to be linear regression.

As a result of testing the model on the test sample, the target RMSE metric value was 34.50. This is below the required threshold of 48.


---
# Предсказание заказов такси на следующий час

### Использованные инструменты

statsmodels, LightGBM, pandas, scikit-learn, Matplotlib

### Ключевые особенности

Временные ряды, регрессия

### Описание задачи

Компания «Чётенькое такси» собрала исторические данные о заказах такси в аэропортах. Чтобы привлекать больше водителей в период пиковой нагрузки, нужно спрогнозировать количество заказов такси на следующий час. Постройте модель для такого предсказания.

Значение метрики _RMSE_ на тестовой выборке должно быть не больше 48.

Вам нужно:

1. Загрузить данные и выполнить их ресемплирование по одному часу.
2. Проанализировать данные.
3. Обучить разные модели с различными гиперпараметрами. Сделать тестовую выборку размером 10% от исходных данных.
4. Проверить данные на тестовой выборке и сделать выводы.

### Общий вывод

В нашем распоряжении оказался временный ряд, содержащий почти 26500 записей. Заметен тренд к увеличению количества заказов со временем.

Провели анализ данных и подготовили детальный вывод. 

Для достижения оптимального результата мы добавили в наш датасет дополнительные признаки: 168-й лаг и 24-х часовое скользящее среднее.

Мы обучили несколько моделей с помощью кросс-валидации и выбрали среди них лучшую. Ею оказалась линейная регрессия. 

В результате проверки модели на тестовой выборке было получено значение целевой метрики RMSE равное 34,50. Это ниже необходимого порога, равного 48. 
