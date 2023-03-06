# Проект «API для Yatube»
Проект даёт возможность работать с проектом Yatube по средством Django REST 
framework.


## Установка и запуск проекта:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/msavilov/api_final_yatube.git
```

Перейти в каталог с проектом

```
cd api_final_yatube
```

Cоздать виртуальное окружение:

```
python3 -m venv env
```

Активировать виртуальное окружение:
Для *nix-систем:

```
source env/bin/activate
```
Для Windows-систем:
```
source env/Scripts/activate
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:
```
python manage.py migrate
```

Запустить проект:
```
python manage.py runserver
```

## Примеры запросов к API

#### Получение публикации по id
Запрос: GET /api/v1/posts/{id}/
Статус ответа: 200 Удачное выполнение запроса
Ответ: 
```
{
    "id": 0,
    "author": "string",
    "text": "string",
    "pub_date": "2019-08-24T14:15:22Z",
    "image": "string",
    "group": 0
}
```

#### Получение публикации по id
Запрос: POST /api/v1/posts/
Статус ответа: 201 Удачное выполнение запроса
Ответ: 
```
{
    "id": 0,
    "author": "string",
    "text": "string",
    "pub_date": "2019-08-24T14:15:22Z",
    "image": "string",
    "group": 0
}
```

