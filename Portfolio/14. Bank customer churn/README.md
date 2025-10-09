# Predicting Customer Churn from a Bank

### Tools Used
scikit-learn, pandas, Matplotlib.

### Key Features
Models: Decision Tree, Random Forest, Logistic Regression. Hyperparameter Selection Using GridSearchCV. Metrics: F1, AUC-ROC. Combating Class Imbalance (class_weight hyperparameter, Upsampling, Downsampling).

### Task Description
Customers have started leaving the bank. Every month. A small, but noticeable, drop. The bank's marketers have calculated that retaining current customers is cheaper than attracting new ones.
We need to predict whether a customer will leave the bank in the near future. We are provided with historical data on customer behavior and contract terminations with the bank.

We need to build a model with the highest possible *F1* score. The target metric value is 0.59. Additionally, we will measure *AUC-ROC* and compare its value with the *F1* measure.

Data source: [https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)

### General conclusion
Data preprocessing was performed. Feature encoding and scaling were performed. Models were trained on an imbalanced sample. Models were trained using various imbalance-mitigation techniques: the class_weight hyperparameter, upsampling, and downsampling. Results were compared, and a conclusion was drawn. The best model was tested. The AUC-ROC metric was analyzed. General conclusions were drawn.


---
# Прогнозирование оттока клиентов из банка

### Использованные инструменты
scikit-learn, pandas, Matplotlib.

### Ключевые особенности
Модели: дерево решений, случайные лес, логистическая регрессия. Подбор гиперпараметров с помощью `GridSearchCV`. Метрики: F1, AUC-ROC. Борьба с дисбалансом классов (гиперпараметр `class_weight`, Upsampling, Downsampling).


### Описание задачи
Из банка стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.
Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Нам предоставлены исторические данные о поведении клиентов и расторжении договоров с банком. 

Необходимо построить модель с предельно большим значением *F1*-меры. Целевое значение метрики - 0.59. Дополнительно измерим *AUC-ROC* и сравним её значение с *F1*-мерой.

Источник данных: [https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)

### Общий вывод
Проведена предобработка данных. Проведено кодирование и масштабирование признаков. Проведено обучение моделей на несбалансированной выборке. Проведено обучение моделей с использованием различных техник борьбы с дисбалансом: гиперпараметр `class_weight`, Upsampling, Downsampling. Сравнили результаты и подготовили вывод. Провели тестирование лучшей модели. Провели исследование метрики AUC-ROC. Сформулировали общий вывод.
