# Бъдещето е код

Сайт на кампанията "Бъдещето е код", популяризираща ползите от умението да се програмира и да се борави с технологии.

## Технически особености

Сайтът е Ruby on Rails приложение. Използва PostgreSQL за база данни. Задвижва се на Heroku.

## Локална инсталация

### Предварителни изисквания

1. Необходимо е да имате инсталиран Ruby интерпретатор. Тук има [инструкции как](http://2014.fmi.ruby.bg/topics/1).
2. Инсталирайте си [Bundler](http://bundler.io/): `gem install bundler`.
3. Трябва да имате достъп до PostgreSQL база данни и потребител с права да създава бази данни.

### Инсталация

1. Клонирайте си хранилището на проекта.
2. Влезте в папката на проекта и инсталирайте зависимостите му с `bundle install`.
3. Копирайте `config/database.yml.example` в `config/database.yml` и го редактирайте с данни за достъп до вашата PostgreSQL инсталация.
4. Копирайте `.env.example` в `.env` и го редактирайте, за да съдържа коректните данни.
5. Изпълнете `bin/rake db:setup` за да създадете база данни с необходимите таблици.
6. Стартирайте `bin/rails server` от директорията на проекта.

На този етап би трябвало да имате работеща локална версия на адрес [localhost:3000](http://localhost:3000).

На [localhost:3000/admin](http://localhost:3000/admin) има административен интерфейс. Потребителското име е `admin@example.com`, а паролата `password`.

## Лиценз

Кодът на това приложение се разпространява под [MIT лиценз](LICENSE.txt).
