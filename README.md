\# Stocks Products API (Docker)



Django REST API проект «Склады и запасы», упакованный в Docker.



\## Технологии



\- Python 3.11

\- Django 3.2

\- Django REST Framework

\- SQLite (для запуска в контейнере)

\- Docker







\## Типовые команды



\### Сборка образа



```bash

docker build -t stocks-api .



Запуск контейнера

bash

docker run -d -p 8000:8000 --name stocks-container stocks-api

Проверка работы

Открой в браузере:



API Root: http://localhost:8000/api/v1/



Товары: http://localhost:8000/api/v1/products/



Остатки: http://localhost:8000/api/v1/stocks/



Админка: http://localhost:8000/admin/



Просмотр логов

bash

docker logs stocks-container

Остановка контейнера

bash

docker stop stocks-container

Удаление контейнера

bash

docker rm stocks-container

Удаление образа

bash

docker rmi stocks-api

