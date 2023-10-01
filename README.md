# _Kittygram_
## О проекте
>Киттиграмм - это социальная сеть для выставления профилей котиков

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
- Запустите сервер с помощью ssh -i путь_до_SSH_ключа/название_файла_с_SSH_ключом_без_расширения login@ip
- Создайте на сервере папку kittygram:
```
mkdir kittygram
```
- Скопируйте из папки проекта файлы docker-compose.production.yml и .env в папку kittygram
- С помощью git actions запустите процесс деплоя

## Отличие версий
Это production-версия проекта kittygram (https://github.com/oleffr/infra_sprint1). В этой версии настроена автомазация при помощи docker и git actions

## Использованные пакеты приложений

>Django                        3.2.3
django-templated-mail         1.1.1
djangorestframework           3.12.4
djangorestframework-simplejwt 4.8.0
pip                           22.0.2
pluggy                        0.13.1
py                            1.11.0
PyJWT                         2.8.0
pytest                        6.2.4
pytest-django                 4.4.0
pytest-pythonpath             0.7.3
python-dotenv                 1.0.0
requests                      2.31.0
requests-oauthlib             1.3.1

## Об Авторе
Автор: Ольга Ефремова (github.com/oleffr)

![example workflow](https://github.com/oleffr/kittygram_final/actions/workflows/main.yml/badge.svg)
