
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
