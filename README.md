# Виявлення маски - Yolov4 модель - Виявлення об'єктів

Модель detect_mask для бібліотеки [yolov4](https://github.com/AlexeyAB/darknet)

> Read this in other language: [Український](README.md), [English](README.en.md), [Русский](README.ru.md)

## Вимоги
* python3
* yolov4

## Навчання
```sh
./darknet detector train data/mask.data data/mask.cfg yolov4.conv.137 -dont_show -map
```

## Виявлення
```sh
./darknet detector test data/mask.data data/mask_test.cfg model/mask.weights data/obj/0.jpg -thresh 0.3
```

## Google colab
```sh
yolov4.ipynb
```

## Приклади
![example_1](https://github.com/martinjack/detect_mask/blob/master/examples/mask.png?raw=true)
![example_1](https://github.com/martinjack/detect_mask/blob/master/examples/nomask.png?raw=true)

# Подяка
* [Yolov4](https://github.com/AlexeyAB/darknet)

* [Kaggle dataset](https://www.kaggle.com/datasets/techzizou/labeled-mask-dataset-yolo-darknet)