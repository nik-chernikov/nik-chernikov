# Comment Classification with BERT

### Tools Used

PyTorch, BERT, CUDA, pandas, NumPy, Matplotlib, scikit-learn

### Key Features

Natural Language Processing (NLP), Text Classification

### Task Description

The Wikishop online store is launching a new service. Now, users can edit and supplement product descriptions, similar to wiki communities. That is, customers offer their edits and comment on others' changes. The store needs a tool that will search for toxic comments and send them for moderation.

Train a model to classify comments as either positive or negative. You have a dataset with edit toxicity markup.

Build a model with an F1 quality metric value of at least 0.75.

### General Conclusion

We have a dataset of 160,000 English-language tweets at our disposal. We needed to train a model that would determine the toxicity of a tweet and have an F1-score metric value of at least 0.75.

We prepared a sample and tokenized the text of the tweets. Then, using the unitary/toxic-BERT model, we created embeddings from the tokens.

We trained 3 different models using GridSearchCV: logistic regression, random forest, and LightGBM. The random forest model showed the best result.

Having tested the random forest model on the test sample, we obtained an F1-score metric value of 0.96183. This is higher than the required minimum result of 0.75. The project goal is achieved.


---  
# Классификация комментариев с BERT

### Использованные инструменты

PyTorch, BERT, CUDA, pandas, NumPy, Matplotlib, scikit-learn

### Ключевые особенности

Обработка естественных языков (NLP), классификация текстов

### Описание задачи

Интернет-магазин «Викишоп» запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Магазину нужен инструмент, который будет искать токсичные комментарии и отправлять их на модерацию.

Обучите модель классифицировать комментарии на позитивные и негативные. В вашем распоряжении набор данных с разметкой о токсичности правок.

Постройте модель со значением метрики качества F1 не меньше 0.75.

### Общий вывод

В нашем распоряжении оказался датасет состоящий из 160000 англоязычных твитов. Нам необходимо было обучить модель, которая бы определяла токсичность твита и имела бы значение метрики f1-score не ниже 0.75. 

Мы подготовили выборку и токенизировали текст твитов. Затем с помощью модели unitary/toxic-bert мы создали из токенов эмбеддинги.

Мы обучили 3 различных модели с использованием GridSearchCV: логистическую регрессию, cлучайный лес и LightGBM. Наилучший результат показала модель случайного леса.

Проверив модель случайного леса на тестовой выборке мы получили значение метрики f1-score равное 0.96183. Это выше требуемого минимального результата в 0.75. Цель проекта выполнена.


