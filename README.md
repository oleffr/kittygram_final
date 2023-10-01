# _Kittygram_
## О проекте
>Киттиграмм (https://github.com/oleffr/kittygram_final) - это социальная сеть для выставления профилей котиков

## Запуск проекта
- Склонируйте репозиторий проекта (https://github.com/oleffr/kittygram_final):
```
 git clone git@github.com:oleffr/kittygram_final.git
```
- - Установите зависимости из файла requirements.txt:
```
 cd kittygram_final/backend
 python3 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
```
- Запустите Docker Compose
```
docker compose -f docker-compose.production.yml up
```
- Cоберите статику
```
docker compose -f docker-compose.production.yml exec backend python manage.py collectstatic
docker compose -f docker-compose.production.yml exec backend cp -r /app/collected_static/. /backend_static/static/
```
- Примените миграции
```
docker compose -f docker-compose.production.yml exec backend python manage.py migrate
```

## Отличие версий
Это (https://github.com/oleffr/kittygram_final) production-версия проекта kittygram (https://github.com/oleffr/infra_sprint1). В этой версии настроена автомазация при помощи docker и git actions

## Использованные пакеты приложений

>Django                       3.2.3
djangorestframework           3.12.4
postgres                      13.10

## Об Авторе
Автор: Ольга Ефремова (github.com/oleffr)

![example workflow](https://github.com/oleffr/kittygram_final/actions/workflows/main.yml/badge.svg)
