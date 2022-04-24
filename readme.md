## Text classification

Входные файлы *train.csv* и *test.csv* можно либо заранее положить 
в дирректорию `dataset`, либо указать их при запуске контейнера.

Предсказание и метрики модели создаются в дирректории `results` образа.

Инструкция по запуску:
1) Собираем докер образ
```
docker build --tag some_name .
```
2) Запускаем образ:
```
docker run some_name
```
3) или
```
docker run -v some_path/train.csv:/app/dataset/train.csv -v some_path/test.csv:/app/dataset/test.csv some_name 
```