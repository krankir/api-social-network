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
- /api/v1/posts/ (**POST**)- Добавление новой публикации.
- /api/v1/posts/{id}/ (**PUT**)- Редактирование публикации.
- ...