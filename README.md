# Итоговый отчет о проделанной работе

## Разработка telegram-бота, по рекомендации фильмов

### Описание проекта

Был разработан Telegram-бот, предоставляющий пользователям персонализированные рекомендации фильмов на основе их предпочтений по жанрам. Пользователь взаимодействует с ботом через кнопки и команды, выбирает жанры и получает список фильмов с высокими рейтингами. Проект сочетает интерактивность и удобство, предоставляя рекомендации в удобном формате.

### Стек

#### Язык программирования:Python
#### Библиотеки:
##### pandas - для работы с данными: загрузка, обработка и анализ.
##### numpy - для работы с числовыми данными и массивами.
##### scikit-learn - для ценки точности предсказаний
##### scipy - для реализации SVD через svds.
##### telegram и telegram.ext - для создания Telegram-бота и обработки взаимодействий с пользователями.
##### math - для вычисления квадратного корня в метрике RMSE.
### Реализованный функционал
#### 1.Рекомендации по жанрам:

Поддерживаются жанры, такие как Драма, Комедия, Фантастика, Триллер и другие.
Пользователь может просматривать топ-10 фильмов по выбранному жанру.
#### 2.Кнопки и команды:

Кнопки для выбора жанра, обновления списка рекомендаций или просмотра следующих фильмов.
Команда /start для приветствия и начала взаимодействия.
#### 3.Алгоритмы рекомендаций:

Memory-Based Collaborative Filtering: Для предсказания рейтингов фильмов на основе данных о пользователях.
SVD (Singular Value Decomposition): Для улучшения точности рекомендаций.
#### 4.Обработка исключений:

Бот уведомляет, если невозможно предоставить рекомендации.
#### 5.Предусмотрена защита от ошибок ввода.

### Запуск и настройка
#### Установка зависимостей:
1. ` pip install python-telegram-bot pandas numpy scikit-learn scipy `

2. Замена токена в коде на токен, полученный от BotFather.
   
3. Запуск бота:
`python bot_script.py`

### Разработка и подготовка данных для модели
#### Загрузка данных:

Данные взяты из набора ml-latest-small, содержащего информацию о фильмах и рейтингах пользователей.
#### Очистка и подготовка:

Обработка и масштабирование идентификаторов фильмов.

Создание пользовательско-фильмовой матрицы для обучения.
#### Модели:

Memory-Based алгоритм и SVD.

Метрика RMSE использована для оценки точности модели.

### Улучшения и изменения
#### Добавление приветственного сообщения:

При запуске бот приветствует пользователя и предоставляет инструкции.

#### Интерактивные кнопки:
Упрощено взаимодействие через Inline-кнопки для выбора жанра и обновления рекомендаций.
#### Гибкость рекомендаций:

Возможность пролистывания фильмов, чтобы подобрать подходящий.
#### Персонализация:

Учитываются предпочтения пользователя, чтобы рекомендации были релевантными.


## Результаты
Telegram-бот создан и выполняет все свои функции.

Реализованы дополнительные функции для улучшения взаимодействия с пользователями.
