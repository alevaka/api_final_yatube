# api_final
api final
### Описание проекта:
  Этот проект представляет собой пример доступа к сервису постов по API, созданному на базе Django REST framework.

### Стек технологий:
 + Python 3
 + Django 2.2.16
 + pytest 6.2.4
 + pytest-pythonpath 0.7.3
 + pytest-django 4.4.0
 + djangorestframework 3.12.4
 + djangorestframework-simplejwt 4.7.2
 + Pillow 8.3.1
 + PyJWT 2.1.0
 + requests 2.26.0

### Примеры запросов:
```
GET к /api/v1/posts/
```
предоставит все посты на сервере
```
POST к /api/v1/posts/
```
с ключом text и необязательными ключами image и group создаст пост от имени залогиненного пользователем
```  
GET к /api/v1/posts/{id}/
```
покажет конкретный пост, а 
```
GET к /api/v1/posts/{id}/comments/
```
комментарии к нему.
И множество других запросов. Полная версия документации доступна в ```/redoc/``` после установки проекта.
### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone git@github.com:alevaka/api_final_yatube.git
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
python -m venv env
```

```
source env/Scripts/activate
```

Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

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
