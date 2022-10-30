# Курс 5. Курсовая

**Краткое описание задачи**

Задание представляет собой маленькую игру с веб-интерфейсом о битве героев в стиле олдскульных браузерных игр.

<details><summary><strong>Знания, необходимые для разработки проекта</strong></summary>

- [ ]  Основы объектно-ориентированного программирования.
- [ ]  Работа с датаклассами.
- [ ]  Навыки функционального программирования, 
использование библиотек marshmallow и marshmallow_dataclasses.
- [ ]  Основы типизации данных.
- [ ]  Работа с данными в  формате JSON.
- [ ]  Основы работы с Flask, использование шаблонов во Flask.
- [ ]  Основы работы с Docker и nginx
</details>

<details><summary><strong>Как работает готовый проект – “флоу” проекта</strong></summary>

1. При переходе на основную страничку с игрой пользователь видит название и кнопку **«Начать игру»** (используем шаблон `index.html`).
2. При нажатии кнопки «Начать игру» пользователь переходит по адресу `/choose-hero/`.

На экране появляется форма, которая принимает следующие данные 
(используем шаблон `choose-hero.html`):

- Название страницы (тег `h2`) («Выберите героя» или «Выберите врага»).
- Предложение ввести имя героя (тег `input`).
- Предложение выбрать класс героя (тег`select`), сформированный на основе названий классов, доступных в программе.
- Предложение выбрать оружие (тег`select`), сформированный на основе имеющихся видов оружия, доступных в программе (исходя из сведений файла `equipment.json`, находится в папке data).
- Предложение выбрать броню (тег`select`), сформированный на основе имеющихся видов брони, доступных в программе (также исходя из сведений файла `equipment.json`).
- Кнопка для отправки заполненных данных.
</details>

---
### Запуск сервера

#### Bash (Linux/MACOS)

```python
export FLASK_APP=run.py
export FLASK_ENV='development'
flask run
```

#### CMD (Windows)

```python
set FLASK_APP=run.py
set FLASK_ENV=development
flask run
```

#### PowerShell (Windows)

```python
$env:FLASK_APP = "run"
$env:FLASK_ENV = "development"
flask run
```
