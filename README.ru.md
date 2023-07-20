# Обнаружение маски - Yolov4 модель - Обнаружение объекта

Модель detect_mask для библиотеки [yolov4](https://github.com/AlexeyAB/darknet)

> Read this in other language: [Український](README.md), [English](README.en.md), [Русский](README.ru.md)

## Требования
* python3
* yolov4

## Обучение
```sh
./darknet detector train data/mask.data data/mask.cfg yolov4.conv.137 -dont_show -map
```

## Обнаружение
```sh
./darknet detector test data/mask.data data/mask_test.cfg model/mask.weights data/obj/0.jpg -thresh 0.3
```

## Google colab
```sh
yolov4.ipynb
```

## Примеры
![example_1](https://github.com/martinjack/detect_mask/blob/master/examples/mask.png?raw=true)
![example_1](https://github.com/martinjack/detect_mask/blob/master/examples/nomask.png?raw=true)

# Спасибо
* [Yolov4](https://github.com/AlexeyAB/darknet)

* [Kaggle dataset](https://www.kaggle.com/datasets/techzizou/labeled-mask-dataset-yolo-darknet)