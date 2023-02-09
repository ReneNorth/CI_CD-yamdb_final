# yamdb_final
Учебный проект по настройке CI/CD через Gitgub actions для API yamdb

![yamdb CI CD](https://github.com/ReneNorth/CI_CD-yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)

### Технологии 

- Python 3.9 
- Django 2.2 
- gunicorn
- Docker
- nginx
- postgreSQL
- psycopg2-binary

### Примеры запросов к API Yambd 

Регистрация на сервисе:  

``` 

http://127.0.0.1:8000/api/v1/auth/singup/ 

``` 

Получение токена:  

``` 

http://127.0.0.1:8000/api/v1/auth/token/ 

``` 

Получение данных через GET-запросы:  

 

- о категориях 

``` 

1. http://127.0.0.1:8000/api/v1/categories/ 

``` 

- о жанрах 

``` 

1. http://127.0.0.1:8000/api/v1/genres/ 

2. http://127.0.0.1:8000/api/v1/genres/{slug}/ 

``` 

- о произведениях 

``` 

1. http://127.0.0.1:8000/api/v1/titles/ 

2. http://127.0.0.1:8000/api/v1/titles/{titles_id}/ 

``` 

- об отзывах на произведениям 

``` 

1. http://127.0.0.1:8000/api/v1/titles/{title_id}/reviews/ 

2. http://127.0.0.1:8000/api/v1/titles/{title_id}/reviews/{review_id}/ 

``` 

- о комментариях к отзывам 

``` 

1. http://127.0.0.1:8000/api/v1/titles/{title_id}/reviews/{review_id}/comments/ 

2. http://127.0.0.1:8000/api/v1/titles/{title_id}/reviews/{review_id}/comments/{comment_id}/ 

``` 

Так же через POST, PUT, PATCH и DELETE-запросы к перечисленным  

эндпоинтам возможно редактирование данных. 

 

Полная документация с определением прав доступа ко всем эндпоинтам  

проекта, примерами содержания запросов и ответов доступна при запущеном  

проекте по адресу:  

``` 

http://127.0.0.1:8000/redoc/ 

``` 
