# Weather App

Создаём приложение, позволяющее смотреть погоду для
определённого местоположения и делиться ссылкой с друзьями.

## NPM Scripts

- `npm run dev` &mdash; запускает Webpack Dev Server и собирает приложение.
  Оно доступно в браузере по адресу `localhost:8080`.
- `npm run build` &mdash; собирает приложение с development настройками.
- `npm run build-prod` &mdash; собирает приложение c production настройками.
- `npm run build-analyze` &mdash; собирает приложение c production настройками
  и показывает сводку о размере бандла приложения в окне браузера.

## Weather API

В качестве API, откуда мы будем получать непосредственно данные о погоде, мы будем
использовать Apixu.

Запросы будут иметь следующий формат:

`GET http://api.apixu.com/v1/current.json?key=e7dea00874ef4735a41104637183004&q=SOME_QUERY`,
где `SOME_QUERY` &mdash; интересующее нас местоположение (например, город).