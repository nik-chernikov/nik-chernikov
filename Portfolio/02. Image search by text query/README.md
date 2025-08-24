# Image search by text query

### Tools used

PyTorch, CUDA, CLIP, transformers, pandas, NumPy, Matplotlib, scikit-learn

### Key features

Computer vision (CV), natural language processing (NLP)

### Task description

You are tasked with developing a demo version of an on-demand image search.

For the demo version, you need to train a model that receives a vector representation of the image and a vector representation of the text, and outputs a value between 0 and 1, indicating how well the text and image match each other.

### General conclusion

We studied the data, prepared it, and trained the neural network model.
The resulting model shows itself slightly better than DummyRegressor.
We also tested the CLIP model from OpenAI. This model does not require training, and it showed excellent results.


---
# Поиск изображения по текстовому запросу

### Использованные инструменты

PyTorch, CUDA, CLIP, transformers, pandas, NumPy, Matplotlib, scikit-learn

### Ключевые особенности

Компьютерное зрение (CV), обработка естественных языков (NLP)

### Описание задачи

Вам поручено разработать демонстрационную версию поиска изображений по запросу.

Для демонстрационной версии нужно обучить модель, которая получит векторное представление изображения, векторное представление текста, а на выходе выдаст число от 0 до 1 — покажет, насколько текст и картинка подходят друг другу.

### Общий вывод

Мы изучили данные, подготовили их и провели обучение модели нейронной сети. 
Полученная модель показывает себя немного лучше, чем DummyRegressor.
Так же мы провели тестирование модели CLIP от OpenAI. Данной модели не требуется обучение и она показала превосходные результаты.


