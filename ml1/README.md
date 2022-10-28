# Лабораторная работа № 1

### Задача

1. Реализовать следующие алгоритмы машинного обучения: Linear/Logistic Regression, SVM, KNN, Naive Bayes в отдельных классах.
2. Данные классы должны наследоваться от BaseEstimator и  ClassifierMixin, иметь методы fit и predict.
3. Вы должны организовать весь процесс предобработки, обучения и тестирования с помощью Pipeline.
4. Вы должны настроить гиперпараметры моделей с помощью кросс валидации, вывести и сохранить эти гиперпараметры в файл, вместе с обученными моделями.
5. Проделать аналогично с коробочными решениями.
6. Для каждой модели получить оценки метрик: Confusion Matrix, Accuracy, Recall, Precision, ROC_AUC curve.
7. Проанализировать полученные результаты и сделать выводы о применимости моделей.
8. Загрузить полученные гиперпараметры модели и обученные модели в формате pickle на гит вместе с jupyter notebook ваших экспериментов.

### Датасет

Для работы был взят датасет из ЛР 0.

### Результаты работы алгоритмов

##### Логистическая регрессия

Подобранные параметры: batch_size: 1000, epochs: 10, learning rate: 0.0001

Оценки метрик:

Accuracy: 0.9150679996397371
Precision: 0.6171581769436997
Recall: 0.06610763310550802

##### Метод опорных векторов

Подобранные параметры: learning rate: 0.001, epochs: 10, batch_size: 1000, alpha: 0.001

Оценки метрик:

Accuracy: 0.9628478789516347
Precision: 0.8874146492861577
Recall: 0.6568835793463902

##### Метод k-ближайших соседей

Подобранные параметры: n_neighbors: 5

Оценки метрик:

Accuracy:  0.9989142073713811
Precision:  0.9955043227665706
Recall:  0.9920165412670151

##### Наивный байесовский классификатор

Оценки метрик:

Accuracy:  0.949538162858887
Precision:  0.7407650847903247
Recall:  0.6472919418758256

### Вывод

Наилучшие результаты показала модель (из коробки), основанная на методе k-ближайших соседей (k = 5), но и работала она дольше всего.ы