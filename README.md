# MAI python projects

## Требования

### Общие требования

[По ссылке](https://docs.google.com/document/d/1nXASx6ALpgiYR-ckc8vap3JsPIWkXILUCbGIk-r_6PQ/edit)
можно получить общие требования к проектам.

#### Перезаписанные требования из ссылки выше

1. > Обязательно должен присутствовать файл requirements.txt
   
    Будем испольовать [pyproject.toml](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) вместо `requirements.txt`
2. > Каждый класс и функция должны быть снабжены DOCSTRING в формате NumpyDoc
   
    Не обязателен формат NumpyDoc. Если хотите использовать другой, укажите это в `README.md`


Также для REST API необходимо иметь [openapi.json](https://spec.openapis.org/oas/latest.html) и `swagger` 
([видео с объяснениями](https://www.youtube.com/watch?v=aaFDBgPdXw4))

(для других видов WEB API необходимо также иметь документацию)

### Git

1. Использовать можно Github/Gitlab/etc.
2. Обязательно должна быть равномерно распределенная история коммитов
3. ci очень желательно(для вашего же удобства), но необязательно
4. cd необязателен
5. Можете(необязательно) настроить pre-commit hook-и
6. Обязательно пригласить меня в репозиторий. ник `sakost` в любой из платформ


### Linters & formatters

1. 1-2 linter-а **обязательно** должны быть (ruff, pylint, flake8)
2. Форматтер по желанию(но для вашего же удобства стоит его настроить) (ruff, black, autoflake)
3. mypy обязателен
4. toml-sort обязателен
5. Можно встроить в ci


### Tests
1. Должны быть unit-test-ы с покрытием кода 50%+
2. e2e и другие тесты по желанию
3. Можно встроить в ci

### poetry
1. Используем [poetry](https://python-poetry.org) для менеджмента зависимостями(собственно, pyproject.toml)
2. Версии указывать необязательно


### Советы

1. Разберитесь с тем, что такое make и Makefile и сделайте там команды для удобства
2. Настройте ci один раз, чтобы каждый раз всё не проверять руками и не ругаться, что в master-е нерабочий код
3. Советую разобраться в лицензировании и добавить лицензию в репозиторий
4. Можете добавить что-то вроде такого ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) в заголовок `README.md`
