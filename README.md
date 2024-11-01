# 3 курс

# Мажирин Александр Алексеевич

# Проектная работа "Веб-ларек"

Стек: HTML, SCSS, TS, Webpack, React

Структура проекта:

- src/ — исходные файлы проекта
- src/components/ — папка с JS компонентами
- src/components/base/ — папка с базовым кодом

Важные файлы:

- src/pages/index.html — HTML-файл главной страницы
- src/types — папка с типами
- src/types — папка с моделями
- src/index.ts — точка входа приложения
- src/scss/styles.scss — корневой файл стилей
- src/utils/constants.ts — файл с константами
- src/utils/utils.ts — файл с утилитами
- src/models/ — папка с моделями

## Установка и запуск

Для установки и запуска проекта необходимо выполнить команды

```
npm install
npm run start
```

или

```
yarn
yarn start
```

## Сборка

```
npm run build
```

или

```
yarn build
```

# Архитектура проекта

## Основные компоненты
Модели: Cart, Product, Order
Представления: CatalogView, ProductView, CartView, OrderView
Контроллеры: CatalogController, ProductController, CartController, OrderController
Брокер событий: EventEmitter

### Описание классов

#### EventEmitter
Класс EventEmitter обеспечивает работу событий. Его функции:

Установить слушателей событий.
Снять слушателей событий.
Вызвать слушателей при возникновении события.

#### Cart
Класс Cart управляет корзиной покупок. Его функции:

Добавить товар в корзину.
Удалить товар из корзины.
Очистить корзину.
Получить общую стоимость товаров в корзине.
Взаимодействие компонентов
Компоненты взаимодействуют через брокер событий EventEmitter, что обеспечивает слабую связанность и масштабируемость системы.
