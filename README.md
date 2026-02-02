# Лендинг whitecore.kz

Одностраничный сайт для AI-Мастерской Whitecore.

## Деплой на Vercel

### Шаг 1: Создать проект в Vercel
1. Зайти на https://vercel.com
2. Нажать "Add New" → "Project"
3. Импортировать из GitHub (или загрузить папку landing)

### Шаг 2: Настройки проекта
- **Framework Preset:** Other
- **Build Command:** (оставить пустым)
- **Output Directory:** . (точка)
- **Install Command:** (оставить пустым)

### Шаг 3: Задеплоить
Нажать "Deploy"

---

## Подключение домена whitecore.kz

### Шаг 1: В Vercel
1. Открыть проект в Vercel
2. Settings → Domains
3. Добавить: `whitecore.kz`
4. Добавить: `www.whitecore.kz`

### Шаг 2: В Unihost (DNS)
Добавить записи:

| Тип | Имя | Значение | TTL |
|-----|-----|----------|-----|
| A | @ | 76.76.21.21 | 3600 |
| CNAME | www | cname.vercel-dns.com | 3600 |

### Шаг 3: Подождать
DNS обновляется 5-30 минут.

---

## Структура

```
landing/
├── index.html      # Главная страница
├── vercel.json     # Конфиг Vercel
└── README.md       # Эта инструкция
```

## Что изменить перед запуском

1. **Логотип/favicon** — заменить emoji на свой логотип
2. **Open Graph картинка** — добавить og:image
3. **Ссылки на документы** — создать /docs/offer.html и /docs/privacy.html

---

**Дата создания:** 2 февраля 2026
