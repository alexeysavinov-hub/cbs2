# Cybersystems VAD LTD — сайт студии (Color Block)

Статический сайт, без сборки и зависимостей. Готов к публикации на любом хостинге (FTP) или GitHub Pages.

## Структура

- `index.html` — сайт (жёлтая версия Color Block)
- `privacy.html`, `terms.html` — Privacy Policy и Terms of Use (ссылки в футере)
- `assets/` — арты Crown Dawn и Merge Arena, скриншоты, иконки и фавиконки, фото офиса, логотип (`logo-mark.svg` — знак, `logo-lockup.svg` — знак с надписью, `favicon.svg` / `favicon-32.png` / `apple-touch-icon.png`, `og.png` — превью для соцсетей)
- `.nojekyll` — отключает обработку Jekyll на GitHub Pages

Разделы: Our Games · About Us · Contact.

## Публикация по FTP

Загрузите содержимое папки (`index.html`, `privacy.html`, `terms.html`, `assets/`) в корень сайта — обычно `public_html/`, `www/` или `htdocs/`. Ничего собирать и настраивать не нужно; файлы `README.md` и `.nojekyll` можно не загружать.

## Публикация на GitHub Pages

1. Загрузите содержимое этой папки в корень ветки `main`.
2. Settings → Pages → Source: **Deploy from a branch** → `main` / `/ (root)` → Save.
3. Сайт появится по адресу `https://<user>.github.io/<repo>/`.
4. Свой домен: добавьте файл `CNAME` с доменом и настройте DNS по инструкции GitHub.

## Что заполнить перед запуском

- **Домен для превью ссылок** — в `<meta property="og:image">` стоит `https://cybersystems.pro/assets/og.png`; замените домен на реальный адрес сайта (картинка `assets/og.png` уже готова).

- **Ссылка на Google Play** — в начале `index.html` впишите её в `window.PLAY_STORE_URL = "";`. Пока ссылки нет, на сайте показывается плашка «Coming soon to Google Play» и статус «In development».
- **Официальный бейдж Google Play** — когда появится ссылка, скачайте бейдж «Get it on Google Play» (English, generic) на https://play.google.com/intl/en_us/badges/ и сохраните его как `assets/google-play-badge.png` (без изменений — так требуют правила Google). Скрипт сам подставит бейдж со ссылкой во все места, где сейчас стоит «Coming soon».
- **Статус игры** — надпись «In development» (плашка в hero и таблица Details) и плашка «Coming soon to Google Play» на баннере: обновите вручную после релиза.
- **Privacy Policy** (`privacy.html`) — раздел 4 «Our games» описывает типовой набор данных F2P-игры; пункты с пометкой **confirm** сверьте с реальными SDK в сборке (аналитика, реклама, крэш-репорты) и удалите пометки. Этот же URL укажите в Play Console как Privacy Policy.
- **Terms of Use** (`terms.html`) — общие условия сайта; проверьте формулировки.
- Шрифты подключаются с Google Fonts — для полной автономности скачайте их в `assets/fonts` и замените `<link>` на `@font-face`.
