# Accident risk assessment

### Tools used

PostgreSQL, SQLAlchemy, pandas, scikit-learn, LightGBM, seaborn, Matplotlib

### Key features

Databases, feature synthesis

### Task description

You are a Data Science specialist at a car-sharing company. You have received an order: you need to create a system that could assess the risk of an accident along a selected route. Risk is understood as the probability of an accident with any damage to the vehicle. As soon as the driver has booked a car, got behind the wheel, and selected a route, the system must assess the risk level. If the risk level is high, the driver will see a warning and recommendations for the route.
The idea of creating such a system is at the stage of preliminary discussion and development. A clear algorithm for work and similar solutions do not yet exist on the market. The current task is to understand whether it is possible to predict accidents based on historical data of one of the regions.

The customer's solution idea:

1. Create a model for predicting road accidents (target value — at_fault (culprit) in the parties table)
   1. For the model, select the culprit type — only a car.
   2. Select cases where the accident resulted in any damage to the vehicle, except for the SCRATCH type.
   3. For modeling, limit yourself to data for 2012 — they are the most recent.
   4. A mandatory condition is to take into account the age of the car.
2. Based on the model, study the main factors of road accidents.
3. Understand whether the modeling results and analysis of the importance of factors will help answer the questions:
   1. Is it possible to create an adequate system for assessing driver risk when issuing a car?
   2. What other factors should be taken into account?
   3. Is it necessary to equip the car with any sensors or a camera?

The customer suggests that you work with the incident database and formulate your own ideas for creating such a system.

### General conclusion

We conducted statistical analysis, checked all the features, and eventually received a dataset of 12 features (including the target) and almost 46 thousand records.

After that, we trained several models and found the best one among them: LightGBM with F1-score = 0.57937.

It is possible to create an adequate model that predicts the risk of an accident before issuing a car, but it is necessary to conduct a study on the selection of the necessary features.

The quality of the model's predictions is far from optimal 0.8-0.9. Probably, having more diverse and more balanced historical data, we could predict the probability of an accident better.


---
# Оценка риска ДТП

### Использованные инструменты

PostgreSQL, SQLAlchemy, pandas, scikit-learn, LightGBM, seaborn, Matplotlib

### Ключевые особенности

Базы данных, синтез признаков

### Описание задачи

Вы — специалист по Data Science в каршеринговой компании. Вам поступил заказ: нужно создать систему, которая могла бы оценить риск ДТП по выбранному маршруту движения. Под риском понимается вероятность ДТП с любым повреждением транспортного средства. Как только водитель забронировал автомобиль, сел за руль и выбрал маршрут, система должна оценить уровень риска. Если уровень риска высок, водитель увидит предупреждение и рекомендации по маршруту.
Идея создания такой системы находится в стадии предварительного обсуждения и проработки. Чёткого алгоритма работы и подобных решений на рынке ещё не существует. Текущая задача — понять, возможно ли предсказывать ДТП, опираясь на исторические данные одного из регионов.

Идея решения задачи от заказчика: 

1. Создать модель предсказания ДТП (целевое значение — at_fault (виновник) в таблице parties)
    1. Для модели выбрать тип виновника — только машина (car).
    2. Выбрать случаи, когда ДТП привело к любым повреждениям транспортного средства, кроме типа SCRATCH (царапина).
    3. Для моделирования ограничиться данными за 2012 год — они самые свежие.
    4. Обязательное условие — учесть фактор возраста автомобиля.
2. На основе модели исследовать основные факторы ДТП.
3. Понять, помогут ли результаты моделирования и анализ важности факторов ответить на вопросы:
    1. Возможно ли создать адекватную систему оценки водительского риска при выдаче авто?
    2. Какие ещё факторы нужно учесть?
    3. Нужно ли оборудовать автомобиль какими-либо датчиками или камерой?

Заказчик предлагает вам поработать с базой данных по происшествиям и сформировать свои идеи создания такой системы. 

### Общий вывод

Мы провели статистический анализ, проверили все признаки и в итоге получили датасет из 12 признаков (включая целевой) и почти 46 тысяч записей.

После этого мы обучили несколько моделей и нашли среди них лучшую: LightGBM с F1-score = 0.57937.

Создать адекватную модель, предсказывающую риск ДТП перед выдачей авто возможно, но требуется провести исследование по подбору необходимых признаков.

Качество предсказаний модели далеко от оптимальных 0.8-0.9. Вероятно имея более разнообразные и более сбалансированные исторические данные, мы могли бы предсказывать вероятность ДТП лучше.
