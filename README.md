# isayevatherapy.com

Сайт Юлии Исаевой — психолога, гештальт-терапевта. Astro + Tailwind, хостинг на GitHub Pages.

## Структура

- `src/pages/index.astro` — главная
- `src/pages/articles/*.astro` — статьи по темам
- `src/layouts/` — общий каркас страницы и шаблон статьи
- `src/styles/global.css` — цвета и стили
- `public/images/yulia.jpg` — фото
- `public/CNAME` — домен для GitHub Pages

## Локальный запуск

```bash
npm install
npm run dev
```

## Публикация

Любой push в ветку `main` автоматически собирает и публикует сайт (`.github/workflows/deploy.yml`).

## DNS для isayevatherapy.com

У регистратора домена:

| Тип   | Имя | Значение              |
|-------|-----|-----------------------|
| A     | @   | 185.199.108.153       |
| A     | @   | 185.199.109.153       |
| A     | @   | 185.199.110.153       |
| A     | @   | 185.199.111.153       |
| CNAME | www | yuisayeva-cpu.github.io |

Затем в репозитории: Settings → Pages → Source: GitHub Actions; Custom domain: `isayevatherapy.com`; включить Enforce HTTPS.
