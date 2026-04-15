Схема тегів:

* **`<body>`** (Фон сторінки)
    * **`<header>`** (Шапка) — 🟦 **FLEX: Рядок (Фото + Текст)**
        * `<figure>` (Фотографія) -> `<img>`
        * `<div class="header-content">` (Забирає решту ширини `flex: 1`)
            * `<h1>` (Ім'я) та `<h2>` (Посада)
            * `<div class="header-contacts">` — 🟦 **FLEX: Рядок з перенесенням** -> `<a>` (Контакти)
    * **`<nav>`** (Навігація) — 🟦 **FLEX: Рядок по центру**
        * `<a>` (Посилання на секції)
    * **`<main>`** (Основний контент) — 🔲 **BLOCK: Центрування (`margin: 0 auto`)**
        * **`<section id="about">`** (Про мене) — 🔲 **BLOCK: Текст зверху вниз**
        * **`<section id="experience">`** (Досвід)
            * `<article>` (Кожне місце роботи)
                * `<header>` — 🟦 **FLEX: Рядок (Іконка + Метадані)**
                * `<ul>` (Обов'язки)
        * **`<section id="portfolio">`** (Портфоліо)
            * `<div class="portfolio-grid">` — 🟦 **FLEX: Сітка з 2 колонок (`flex-wrap: wrap`)**
                * `<article>` (Картка проекту) — 🟦 **FLEX: Стовпчик (`flex-direction: column`)**
                    * `<h4>` (Назва) та `<figure>` (Картинка)
                    * `<div class="card-body">` (Забирає решту висоти `flex: 1`) -> Містить `<div class="card-links">` (Кнопки завжди внизу)
        * **`<section id="skills">`** (Навички)
            * `<div class="badges-row">` — 🟦 **FLEX: Рядок з перенесенням (`wrap`)** -> `<span class="skill-badge">`
        * **`<section id="achievements">`** (Досягнення) — 🔲 **BLOCK: Нумерований список** -> `<ol>` -> `<li>`
        * **`<div class="bottom-grid">`** (Нижній блок) — 🟦 **FLEX: 2 рівні колонки**
            * **`<section id="languages">`** (Мови) -> `<dl>` — 🟩 **GRID: Таблиця на 2 колонки (`auto` та `1fr`)**
            * **`<aside>`** (Додатково) — 🔲 **BLOCK: Текст та картинка**
    * **`<footer>`** (Підвал)
        * `<div class="footer-top">` — 🟦 **FLEX: Рядок (Розкидано по краях `space-between`)**
        * `<div class="footer-contacts">` — 🟦 **FLEX: 2 колонки (`flex-wrap: wrap`)** -> `<div class="contact-item">` (Ширина 50%)
        * `<div class="footer-bottom">` — 🟦 **FLEX: Рядок (Розкидано по краях)**