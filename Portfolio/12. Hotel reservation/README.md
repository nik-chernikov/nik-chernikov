# Predicting Customer Churn in a Hotel Chain

### Tools Used
scikit-learn, pandas, NumPy, Matplotlib, seaborn.

### Key Features
Model development and revenue estimation from its implementation.

### Task Description
The client of this study is the hotel chain "Like a Guest".

To attract customers, this hotel chain added the option to book a room without prepayment to its website. However, if a customer canceled a reservation, the company suffered losses. Hotel staff might, for example, overstock on groceries for the guest's arrival or simply be unable to find another customer.

To solve this problem, we need to develop a system that predicts cancellations. If the model predicts a cancellation, the customer is asked to pay a deposit. The deposit is 80% of the one-night room rate and one-time cleaning costs. The deposit will be debited from the customer's account if they cancel.

The proposed metric is the revenue generated after implementing the machine learning model.

### General Conclusion
Preprocessing and exploratory data analysis were performed. Cyclical features, such as day of week and month, were transformed. Redundant features were removed and new ones added. Outliers were processed. An ML problem was formulated based on the business problem. Logistic regression and random forest models were trained, and the best model was selected. A profile of an "unreliable" client was described. A general conclusion was formulated.


---
# Прогнозирование оттока клиентов в сети отелей

### Использованные инструменты
scikit-learn, pandas, NumPy, Matplotlib, seaborn.

### Ключевые особенности
Разработка модели и оценка величины выручки от её внедрения.

### Описание задачи
Заказчик этого исследования — сеть отелей «Как в гостях».

Чтобы привлечь клиентов, эта сеть отелей добавила на свой сайт возможность забронировать номер без предоплаты. Однако если клиент отменял бронирование, то компания терпела убытки. Сотрудники отеля могли, например, закупить продукты к приезду гостя или просто не успеть найти другого клиента.

Чтобы решить эту проблему, нам нужно разработать систему, которая предсказывает отказ от брони. Если модель покажет, что бронь будет отменена, то клиенту предлагается внести депозит. Размер депозита — 80% от стоимости номера за одни сутки и затрат на разовую уборку. Деньги будут списаны со счёта клиента, если он всё же отменит бронь.

В качестве метрики предлагается использовать величину выручки которая получится после внедрения модели машинного обучения.

### Общий вывод
Проведена предобработка и исследовательский анализ данных. Преобразованы цикличные признаки, такие как день недели и месяца. Удалены лишние признаки и добавлены новые. Обработаны выбросы. Сформулирована ML-задача на основе бизнес-задачи. Обучены модели логистической регрессии и случайного леса, выбрана лучшая модель. Описан портрет "ненадёжного" клиента. Сформулирован общий вывод.
