Онлайн - магазин одежды (online shop)

Бэкенд: фрэймворк Express
Запуск: node server/server.js
Сервер в данном проекте является очень простым и хранит в json-файлах (server/db) информацию:
- о продуктах (без url фото продукта; для целей проекта везде использовано фото-заглушка);
- о корзине текущего пользователя (наименование/количество/цена продуктов);
- о статистике действий пользователя (server/db/stats.json)

Фронтенд: фрэймворк Vue.js
Запуск: npm run serve
Пользовательский интерфейс:
    1. Главная страница
    1.0. Хэдер:
        - переход главная/корзина - по клику на значки в верхнем меню
        - значок корзины (при наведении) - открытие меню для просмотра/удаления товаров из корзины
    1.1. Фильтр - поиск по названию товаров, реализован на основе регулярных выражений
    1.2. Карточки товаров:
        - переход на страницу товара - по клику на название товара;
        - добавление товара в корзину - навести мышку на товар / кликнуть на кнопку Add to cart 
    2. Страница товара: просмотр информации о товаре, добавление товара в корзину.
    3.Корзина: добавление в / удаление товаров из корзины

Стили, CSS: верстка страниц осуществлена самостоятельно (без использования Bootstrap и т.п.) на основе Figma-шаблона.