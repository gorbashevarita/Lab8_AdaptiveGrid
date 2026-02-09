# Лабораторная работа №8 по ИСРПО
**Цель работы:** освоить современные технологии CSS-разметки — Grid.
#### Структура проекта
- grid.css
- gridPractice.css
- gridPractice.html
- index.html
- README.md
- папка img

***

#### 1. Базовые примеры `Grid`
- `display: grid`;
- `grid-template-columns`;
- `grid-template-rows`;
- `grid-template-areas`;
- `gap`;
- `justify-content`;
- `align-items`.

#### 2. Практические примеры `Grid`
1. Как сделать базовую сетку 3x2:
HTML:
```html
<div class="container">
  <div>1</div>
  <div>2</div>
  <div>3</div>
  <div>4</div>
  <div>5</div>
  <div>6</div>
</div>
```
CSS:
```css
.container {
  display: grid;
  grid-template-columns: 100px 100px 100px;
  grid-template-rows: 50px 50px;
}
```
2. Как добавить промежутки между элементами

CSS:
```css
.container {
  gap: 20px;
}
```

3. Как задать макет через визуальную сетку имен:

HTML:
```html
<div class="layout">
  <header>Шапка</header>
  <nav>Меню</nav>
  <main>Контент</main>
  <footer>Подвал</footer>
</div>
```
CSS:
```css
.layout {
  display: grid;
  grid-template-areas: 
    "header header"
    "nav main"
    "footer footer";
  grid-template-rows: 60px 1fr 60px;
  grid-template-columns: 20% 1fr;
}
```

#### Сравнение Flexbox и CSS Grid

| Критерий| Flexbox| CSS Grid|
|----|----|----|
| Тип компоновки| Одномерная | Двумерная|
| Управление| Строка **или** столбец| Строки **и** столбцы|
| Основное назначение| Выравнивание элементов| Построение макетов|
| Подходит дляъ| Компонентов| Страниц и сложных сеток |

#### Типичные сценарии использования

| Задача  | Рекомендуется  |
|--|------|
| **Навигационное меню**| Flexbox|
| **Карточки товаров**| Flexbox + Grid |
| **Центрирование элемента** | Flexbox|
| **Макет страницы**| Grid |
| **Галерея изображений** | Grid |
| **Дашборд** | Grid |
***

**Итог:** получены практические навыки для разработки адаптивных интерфейсов с использованием CSS Grid.

*Автор*:
Горбачева Маргарита, ИСП-231