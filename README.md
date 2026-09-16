# Cybersystems VAD LTD — сайт студии

Статический сайт, без сборки и зависимостей. Готов к публикации на GitHub Pages.

## Структура

- `index.html` — основная версия (Night Arcade, тёмная)
- `color-block/index.html` — альтернативная версия (Color Block, светлая)
- `assets/` — арты Crown Dawn, скриншоты, иконка, логотипы партнёров, фото офиса
- `.nojekyll` — отключает обработку Jekyll на GitHub Pages

## Публикация на GitHub Pages

1. Создайте репозиторий и загрузите содержимое этой папки в корень ветки `main`.
2. Settings → Pages → Source: **Deploy from a branch** → `main` / `/ (root)` → Save.
3. Сайт появится по адресу `https://<user>.github.io/<repo>/`, альтернатива — `/color-block/`.
4. Свой домен: добавьте файл `CNAME` с доменом и настройте DNS по инструкции GitHub.

## Что заполнить перед запуском

- **Ссылка на Google Play** — в начале `index.html` (и `color-block/index.html`) впишите её в
  `window.PLAY_STORE_URL = "";` — все кнопки «Get it on Google Play» подхватят её автоматически.
- **Статус игры** — надпись «In development» в тексте (hero-плашка и таблица Details).
- **Реквизиты** — Registration No. и VAT No. в блоке Company details замаскированы (`HE ••••••`, `CY••••••••L`).
- **Логотипы партнёров** — файлы `assets/partner-0N-light.png` (тёмная версия) и `assets/partner-0N-dark.png` (светлая); заменяйте, сохраняя имена.
- **Политики** — ссылки Privacy Policy / Terms / Cookie Policy в футере ведут на `#`; подставьте реальные страницы.
- Шрифты подключаются с Google Fonts — для полной автономности скачайте их в `assets/fonts` и замените `<link>` на `@font-face`.
