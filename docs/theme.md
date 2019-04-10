### Доступные готовые темы

Страница со списком тем:
[Ссылка](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Themes)


## Установка темы на примере Material for MkDocs:

### Установка
Ссылка на документацию темы [Material](https://squidfunk.github.io/mkdocs-material/)
Выполним установку темы в командной строке проекта
```console
pip install mkdocs-material
```
Добавим установленную тему в настроечный файл ```mkdocs.yml```:
```yaml
theme:
  name: 'material'
```

Добавим настройку для темы, а также добавим дополнения.  
Создадим блок ```nav``` для создания структурированного меню.  
В поле plugins>search>lang укажем языки доступные через поиск  
Для текущей темы необходимо выставить языки поиска отдельно, в поле extra  
И перечислим подключаемые плагины для темы в графе markdown_extensions  
Инструкции по плагинам можно найти [здесь](https://squidfunk.github.io/mkdocs-material/extensions/admonition/)  
```yaml
site_name: Пример документации
repo_url: https://sampledocumentation.readthedocs.io
nav:
    - Описание: index.md
    - Установка и настройка MKDocks: install.md
    - Установка и настройка тем: theme.md
plugins:
    - search:
        lang: [ru, en]
theme:
    name: 'material'
    language: 'ru'
extra:
    search:
        language: 'en, de, ru'
markdown_extensions:
    - codehilite
    - admonition
```



