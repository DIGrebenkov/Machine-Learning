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

Подобранные параметры: batch_size: 1000, epochs: 10, learning rate: 0.001

Оценки метрик:

Accuracy: 0.7100076785257231

Precision: 0.8177458033573142

Recall: 0.5306016597510373

![image](https://user-images.githubusercontent.com/71839146/198822256-11f61d27-9d57-496d-8e87-d5c33affe019.png)

![image](https://user-images.githubusercontent.com/71839146/198822261-5d9de47c-2675-4623-8df2-8e380f7fa8e1.png)

##### Метод опорных векторов

Подобранные параметры: learning rate: 0.001, epochs: 1, batch_size: 1000, alpha: 0.0001

Оценки метрик:

Accuracy: 0.9513693370872792

Precision: 0.9306243805748265

Recall: 0.9740663900414938

![image](https://user-images.githubusercontent.com/71839146/198822268-2cd31831-e4fa-4a81-9790-78a5076e4b2b.png)

![image](https://user-images.githubusercontent.com/71839146/198822273-846215ad-cdf6-4e11-9383-ca4ecd629fb2.png)

##### Метод k-ближайших соседей

Подобранные параметры: k: 1

Оценки метрик:

Accuracy: 0.9948809828512926

Precision: 0.9920061887570912

Recall: 0.9976659751037344

![image](https://user-images.githubusercontent.com/71839146/198822277-81749ce5-71a1-466e-b3d3-c1a916ebf9f8.png)

![image](https://user-images.githubusercontent.com/71839146/198822285-6a9a1f78-53f6-44f0-adc4-08bc3f0d922f.png)

##### Наивный байесовский классификатор

Оценки метрик:

Accuracy: 0.7139749168159714

Precision: 0.6330651781316696

Recall: 1.0

![image](https://user-images.githubusercontent.com/71839146/198822289-d0fbb0d8-ccda-425d-813c-a8a9b6cebba6.png)

![image](https://user-images.githubusercontent.com/71839146/198822291-579f7dc9-1611-4aaa-a220-0a9683503fc6.png)

### Вывод

Наилучшие результаты показала модель, основанная на методе k-ближайших соседей (k = 1).
