# Determining the age of a buyer from a photo

### Tools used

Keras, pandas, Matplotlib

### Key features

Computer vision (CV), image processing

### Task description

The Khleb-Sol supermarket chain is implementing a computer vision system for processing photos of buyers. Photo recording in the checkout area will help determine the age of customers to:

1. Analyze purchases and offer products that may interest buyers of this age group;
2. Monitor the integrity of cashiers when selling alcohol.

Build a model that will determine the approximate age of a person from a photo. You have a set of photos of people with ages at your disposal.

### General conclusion

Exploratory data analysis was conducted. Its results:

1. We have 7591 images of people of different ages at our disposal.
2. The age distribution in the dataset is uneven, with several peaks and dips.
3. The quality of the images is different. But the area occupied by the faces of people in the photo is approximately the same.

Then we trained the ResNet50 model and achieved the target MAE metric on the test equal to 5.9564. This is below the required value of MAE < 8 and below the "excellent" value of MAE < 7.

The last layers of the model were written manually. Additional training of the main ResNet50 model was used. The MSE function was used as a loss function. The Adam algorithm with a learning rate of 0.0001 was used as an optimizer.

The model was trained for 50 epochs, and the target metric was achieved already in the 3rd epoch. First of all, this was achieved by reducing the learning rate of the Adam optimizer to 0.0001. Using the MSE function as a loss function also had a positive effect.

The target metric was achieved, and the task is completed.

The resulting model will help in solving the tasks set by the business. Namely:
1. Analyze purchases and offer products that may be of interest to buyers of this age group;
2. Monitor the integrity of cashiers when selling alcohol.


---
# Определение возраста покупателя по фотографии

### Использованные инструменты

Keras, pandas, Matplotlib

### Ключевые особенности

Компьютерное зрение (CV), обработка изображений

### Описание задачи

Сетевой супермаркет «Хлеб-Соль» внедряет систему компьютерного зрения для обработки фотографий покупателей. Фотофиксация в прикассовой зоне поможет определять возраст клиентов, чтобы:

1. Анализировать покупки и предлагать товары, которые могут заинтересовать покупателей этой возрастной группы;
2. Контролировать добросовестность кассиров при продаже алкоголя.

Постройте модель, которая по фотографии определит приблизительный возраст человека. В вашем распоряжении набор фотографий людей с указанием возраста.

### Общий вывод

Был проведён исследовательский анализ данных. Его результаты:

1. В нашем распоряжении имеется 7591 изображение людей разных возрастов.
2. Распределение по возрастам в датасете неравномерное, с несколькими пиками и провалами.
3. Качество изображений различное. Но при этом площадь, которую занимают лица людей на фото примерно одинакова.

Затем мы обучили модель ResNet50 и добились целевой метрики MAE на тесте, равной 5.9564. Это ниже необходимого значения MAE < 8 и ниже "отличного" значения MAE < 7.

Последние слои модели были написаны вручную. Применялось дообучение основной модели ResNet50. В качестве loss-функции использовалась функция MSE. В качестве оптимизатора использовался алгоритм Adam c learning rate = 0.0001.

Модель была обучена в течении 50 эпох, целевой показатель метрики был достигнут уже на 3-ей эпохе. В первую очередь, этого удалось достигнуть благодаря уменьшению скорости обучения оптимизатора Adam до 0.0001. Так же положительно сказалось использование в качестве функции потерь функции MSE.

Целевая метрика достигнута, задача выполнена.

Полученная модель поможет в решении задач, поставленных бизнесом. А именно:
1. Анализировать покупки и предлагать товары, которые могут заинтересовать покупателей этой возрастной группы;
2. Контролировать добросовестность кассиров при продаже алкоголя.


