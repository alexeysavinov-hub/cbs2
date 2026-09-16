# Cybersystems VAD LTD — сайт студии (Color Block)

Статический сайт, без сборки и зависимостей. Готов к публикации на GitHub Pages.

## Структура

- `index.html` — сайт (жёлтая версия Color Block)
- `assets/` — арты Crown Dawn и Merge Arena, скриншоты, иконка, фото офиса
- `.nojekyll` — отключает обработку Jekyll на GitHub Pages

Разделы: Our Games · About Us · Contact.

## Публикация на GitHub Pages

1. Загрузите содержимое этой папки в корень ветки `main`.
2. Settings → Pages → Source: **Deploy from a branch** → `main` / `/ (root)` → Save.
3. Сайт появится по адресу `https://<user>.github.io/<repo>/`.
4. Свой домен: добавьте файл `CNAME` с доменом и настройте DNS по инструкции GitHub.

## Что заполнить перед запуском

- **Ссылка на Google Play** — в начале `index.html` впишите её в `window.PLAY_STORE_URL = "";` — все кнопки «Get it on Google Play» подхватят её автоматически.
- **Статус игры** — надпись «In development» (плашка в hero и таблица Details).
- **Политики** — ссылки Privacy Policy / Terms / Cookie Policy в футере ведут на `#`; подставьте реальные страницы.
- Шрифты подключаются с Google Fonts — для полной автономности скачайте их в `assets/fonts` и замените `<link>` на `@font-face`.
