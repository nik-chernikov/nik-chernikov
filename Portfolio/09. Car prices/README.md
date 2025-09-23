# Determining the price of cars

### Tools used
LightGBM, scikit-learn, category_encoders, pandas, NumPy, Matplotlib.

### Key features
Gradient boosting.

### Task description
The used car sales service "Ne bit, ne krashen" is developing an app to attract new customers. It enables users to quickly determine the market value of their car. You have access to historical data: technical specifications, configurations, and car prices. You need to build a model to determine the value.

The customer cares about:

- Prediction quality. The RMSE metric should be less than 2500;
- Prediction speed;
- Training time.

### General conclusion
1. Data preprocessing was completed. Anomalies, outliers, and incorrect values were processed.
2. The linear regression and LightGBM models were trained using cross-validation. The optimal hyperparameters for LightGBM were found using GridSearchCV.
3. The trained models were compared in terms of RMSE, training speed, and prediction speed. The LightGBM model trains and predicts more slowly but shows better results in terms of RMSE.
    1. The best model was compared with a constant model.
    2. The best model was tested on a test sample.

The result is a model that meets the customer's criteria and is ready for implementation.


---
# Определение стоимости автомобилей

### Использованные инструменты
LightGBM, scikit-learn, category_encoders, pandas, NumPy, Matplotlib.

### Ключевые особенности
Градиентный бустинг.

### Описание задачи
Сервис по продаже автомобилей с пробегом «Не бит, не крашен» разрабатывает приложение для привлечения новых клиентов. В нём можно быстро узнать рыночную стоимость своего автомобиля. В вашем распоряжении исторические данные: технические характеристики, комплектации и цены автомобилей. Вам нужно построить модель для определения стоимости. 

Заказчику важны:

- Качество предсказания. Величина метрики RMSE должна быть менее 2500;
- Скорость предсказания;
- Время обучения.

### Общий вывод
1. Выполнена предобработка данных. Аномалии, выбросы, некорректные значения были обработаны.
2. Обучены с применением кросс-валидации модели линейной регрессии и LightGBM. Для LightGBM были найдены оптимальные гиперпараметры с помощью `GridSearchCV`.
3. Проведено сравнение обученных моделей по метрике RMSE и скорости обучения и предсказания. Модель LightGBM обучается и предсказывает медленнее, но показывает лучший результат по метрике RMSE.
    1. Проведено сравнение лучшей модели с константной моделью.
    2. Проведена проверка лучшей модели на тестовой выборке.

В результате получена модель, соответствующая критериям заказчика и готовая для внедрения в эксплуатацию.