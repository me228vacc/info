# info — одностраничник для GitHub Pages

Готовый каркас: вставляешь текст одним Ctrl-C Ctrl-V в `index.html`.

## Куда вставлять текст

1. Открой `index.html`.
2. Найди блок:
   ```
   <!-- PASTE-START -->
   ...
   <!-- PASTE-END -->
   ```
3. Удали пример внутри `<div class="paste">...</div>`.
4. Вставь свой текст внутрь этого `div`. Теги не нужны — переносы сохранятся.

Заголовок страницы поменяй в `<h1>` и `<title>`.

## Локальный просмотр

Просто открой `index.html` в браузере. Сборка не нужна.

## Публикация (по quickstart Pages)

Remote уже настроен:
```
origin  https://github.com/me228vacc/info.git (fetch)
origin  https://github.com/me228vacc/info.git (push)
```

1. Создай на GitHub пустой репозиторий `me228vacc/info` (без README, чтобы не было конфликта).
2. Включи Pages: Settings → Pages → Source: Deploy from branch → Branch: `main` / `(root)`.
3. Отправь код:
   ```
   git add index.html assets/style.css .nojekyll README.md
   git commit -m "Init onepage info"
   git push -u origin main
   ```
4. Сайт будет: `https://me228vacc.github.io/info/` (обновление до ~10 минут).

Файл `.nojekyll` нужен, чтобы Pages отдавал чистый HTML без обработки Jekyll.
