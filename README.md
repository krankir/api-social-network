# api_final_yatube
Проект для отработки написания API для сайта
### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/krankir/api_final_yatube.git
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv venv
```

```
source venv/bin/activate
```

Установить зависимости из файла requirements.txt:

```
python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```

### Документация к API проекта:

Перечень запросов к ресурсу можно посмотреть в описании API

```
http://127.0.0.1:8000/redoc/
```

### Примеры запросов

- /api/v1/posts/ (**GET**)- Получить список всех публикаций.

Response samples :
```
[
    {
        "id": 0,
        "author": "string",
        "text": "string",
        "pub_date": "2021-10-14T20:41:29.648Z",
        "image": "string",
        "group": 0
    }
]
```
- /api/v1/posts/ (**POST**)- Добавление новой публикации.

Request sample :
```
{
    "text": "string",
    "image": "string",
    "group": 0
}
```
Response samples :
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
- /api/v1/posts/{id}/ (**PUT**)- Редактирование публикации.

Request sample :
```
{
    "text": "string",
    "image": "string",
    "group": 0
}
```
Response samples :
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
- ...