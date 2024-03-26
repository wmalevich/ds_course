# Monet vs Manet
Классификация картин для выявления их автора
## Создание датасета
* ##### Отбор картин 
Для данной задачи были отобраны одинаково, наиболее популярные и менее известные работы художников. 
В итоге получилось по 54% и 46% картин Моне и Мане соответственно
* ##### Roboflow
Для создания кастомного датасета использовался Roboflow
1. Разметка данных
2. Препроцессинг<br>
![preprocessing](<preprocessing.png>)
   * Auto-Orient
   * Resize
3. Аугментация<br>
![augmentation](<augmentation.png>)
    * Flip
    * Brightness ±20% 
## Обучение в Roboflow
* ##### Обучение
![alt text](roboflow_training1.png)
![alt text](roboflow_training2.png)
* ##### Результаты
![alt text](roboflow_results1.png)
![alt text](roboflow_results2.png)
## Обучение YOLOv5
Для обучения использовалась nano модель YOLO
* ##### Результаты обучения на 30 эпохах
Предсказания на 2 Моне, 1 Мане<br>
![alt text](test_image2(30epochs).png) ![alt text](test_image0(30epochs).png) ![alt text](test_image1(30epochs).png)
* ##### Результаты обучения на 50 эпохах
2 Monet
![alt text](test_image0(50epochs).png) ![alt text](test_image1(50epochs).png)
## Предсказания модели
* ##### Результаты
Похоже, что, переобучение :(





