Taski - это приложение для создания, обновления, мониторинга собственных задач и API для него.
В рамках работы с этим проектом, я учился деплою веб-приложений в рабочей среде.

#  Как работать с репозиторием финального задания

## Что нужно сделать

Настроить запуск проекта Taski в контейнерах и CI/CD с помощью GitHub Actions

## Как проверить работу с помощью автотестов

В корне репозитория создайте файл tests.yml со следующим содержимым:
```yaml
repo_owner: ваш_логин_на_гитхабе
taski_domain: полная ссылка (https://доменное_имя) на ваш проект Taski
dockerhub_username: ваш_логин_на_докерхабе
```

Для локального запуска тестов создайте виртуальное окружение, установите в него зависимости из backend/requirements.txt и запустите в корневой директории проекта `pytest`.

## Чек-лист для проверки перед отправкой задания

- Проект Taski доступен по доменному имени, указанному в `tests.yml`.
- Пуш в ветку main запускает тестирование и деплой Taski, а после успешного деплоя вам приходит сообщение в телеграм.

