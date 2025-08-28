# Predicting the temperature of a star

### Tools used
PyTorch, category_encoders, pandas, Matplotlib, NumPy.

### Key features
Fully connected feedforward neural networks (FNN).

### Task description
We received a task from the Sky in the Palm observatory: to figure out how to use a neural network to determine the surface temperature of discovered stars. Scientists usually use the following methods to calculate the temperature:

- Wien's displacement law.
- Stefan-Boltzmann law.
- Spectral analysis.

Each of them has its pros and cons. The observatory wants to implement machine learning technologies to predict the temperature of stars, hoping that this method will be the most accurate and convenient. The observatory's database contains characteristics of 240 stars that have already been studied.

The target metric is RMSE. It should not exceed 4500.

### General conclusion
Data preprocessing has been performed. Several neural networks have been created and trained; the optimal number of layers and neurons has been selected. The selected neural network has been trained with various combinations of DropOut and BatchNorm. Such hyperparameters as learning rate and batch size have been selected. An acceptable result of the control metric has been obtained.

### What can be improved
1. The dataset has a strong imbalance. You can try to synthesize the missing classes using libraries such as SMOTE.

2. Use the Scorch library to select optimal hyperparameters.


---
# Прогнозирование температуры звезды

### Использованные инструменты
PyTorch, category_encoders, pandas, Matplotlib, NumPy.

### Ключевые особенности
Полносвязные нейросети прямого распространения (FNN).

### Описание задачи
Нам пришла задача от обсерватории «Небо на ладони»: придумать, как с помощью нейросети определять температуру на поверхности обнаруженных звёзд. Обычно для расчёта температуры учёные пользуются следующими методами:

- Закон смещения Вина.
- Закон Стефана-Больцмана.
- Спектральный анализ.

Каждый из них имеет плюсы и минусы. Обсерватория хочет внедрить технологии машинного обучения для предсказания температуры звёзд, надеясь, что этот метод будет наиболее точным и удобным. В базе обсерватории есть характеристики уже изученных 240 звёзд.

Целевая метрика - RMSE. Она не должна превышать 4500.

### Общий вывод
Проведена предобработка данных. Созданы и обучены несколько нейросетей, выбрано оптимальное количество слоёв и нейронов. Выбранная нейросеть обучена с различными комбинациями DropOut и BatchNorm. Проведён подбор таких гиперпараметров как скорость обучения и размер батча. Получен приемлимый результат контрольной метрики.

### Что можно улучшить
1. Датасет имеет сильный дисбаланс. Можно попробовать синтезировать недостающие классы с помощью таких библиотек, как SMOTE. 
2. Использовать библиотеку Scorch для подбора оптимальных гиперпараметров.
