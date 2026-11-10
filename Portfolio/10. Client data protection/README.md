# Protecting Client Personal Data

### Tools Used
scikit-learn, pandas, NumPy.

### Key Features
It has been proven that multiplying features by an invertible matrix does not change the model's predictions.

### Task Description
We need to protect the data of clients of the insurance company "Even if there is a flood". We need to develop a data transformation method that makes it difficult to recover personal information from it. We need to justify its correct operation.

We need to protect the data so that the quality of machine learning models does not degrade during the transformation. Selecting the best model is not required.

### General Conclusion  
The following problem has been formulated and solved:

> Features are multiplied by an invertible matrix. Will the quality of the linear regression change?
> 1. It will change. In this case, please provide examples of matrices.
> 2. It will not change. In this case, it is necessary to indicate how the linear regression parameters in the original problem and in the transformed one are related.

It has been proven that multiplying features by an invertible matrix helps encrypt the data and does not affect the value of the R2 metric.


---
# Защита персональных данных клиентов

### Использованные инструменты
scikit-learn, pandas, NumPy.

### Ключевые особенности
Доказано, что умножение признаков на обратимую матрицу не приведёт к изменению предсказаний модели.

### Описание задачи
Нам нужно защитить данные клиентов страховой компании «Хоть потоп». Необходимо разработать такой метод преобразования данных, чтобы по ним было сложно восстановить персональную информацию. Необходимо обосновать корректность его работы.

Нужно защитить данные, чтобы при преобразовании качество моделей машинного обучения не ухудшилось. Подбирать наилучшую модель не требуется.

### Общий вывод
Сформулирована и решена следующая задача:

> Признаки умножают на обратимую матрицу. Изменится ли качество линейной регрессии?
> 1. Изменится. В таком случае необходимо привести примеры матриц.
> 2. Не изменится. В таком случае необходимо указать, как связаны параметры линейной регрессии в исходной задаче и в преобразованной.

Доказано, что умножение признаков на обратимую матрицу помогает зашифровать данные и не влияет на значение метрики R2.