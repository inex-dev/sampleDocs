### Установка

Установим в наш проект библиотеку mkdocs:
```console
pip install mkdocs
```
### Создание проекта

В созданном проекте выполним команду:
```console
mkdocs new my-project
```

!!! info "Подсказка"
    my-project - имя для создания папки. Для создания папки по умолчанию docks вместо имени проекта my-project просто поставьте точку.

### Запуск проекта

Для запуска созданного проекта выполним команду:
```console
mkdocs serve
```
!!! info "Подсказка"
    Для просмотра документации на сервере перейдите по адресу: http://127.0.0.1:8000

### Настроечный файл mkdocks.yml

mkdocks.yml - это конфигурационный файл для MKDocks. Зададим ему некоторые настройки:
```yaml
site_name: Пример документации
repo_url: https://github.com/example/repository/
nav:
    - Описание: index.md
    - Установка и настройка MKDocks: install.md
    - Установка и настройка тем: theme.md
plugins:
    - search:
        lang: [ru, en]
```
