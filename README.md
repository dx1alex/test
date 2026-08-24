# Directus Project Template

Шаблон проекта для быстрой настройки Directus CMS.

## Структура проекта

```
directus-template/
├── docker-compose.yml      # Docker конфигурация
├── .env                    # Переменные окружения
├── .gitignore             # Git ignore файл
├── README.md              # Документация
└── directus/              # Директория для данных Directus
    ├── database/          # База данных SQLite (если используется)
    └── uploads/           # Загруженные файлы
```

## Быстрый старт

### Вариант 1: Docker (рекомендуется)

1. Скопируйте `.env.example` в `.env` и настройте переменные:
```bash
cp .env.example .env
```

2. Запустите контейнеры:
```bash
docker-compose up -d
```

3. Откройте браузер и перейдите по адресу: `http://localhost:8055`

### Вариант 2: NPM

1. Установите зависимости:
```bash
npm init directus@latest
```

2. Следуйте инструкциям установщика

## Переменные окружения

Основные переменные в `.env`:

- `KEY` - Секретный ключ для JWT
- `SECRET` - Секретный ключ для шифрования
- `DB_CLIENT` - Тип базы данных (sqlite/pg/mysql)
- `DB_FILENAME` - Путь к файлу БД (для SQLite)
- `ADMIN_EMAIL` - Email администратора
- `ADMIN_PASSWORD` - Пароль администратора

## Полезные команды

### Docker
```bash
# Запуск
docker-compose up -d

# Остановка
docker-compose down

# Просмотр логов
docker-compose logs -f

# Перезапуск
docker-compose restart
```

## Документация

- [Официальная документация Directus](https://docs.directus.io/)
- [GitHub репозиторий](https://github.com/directus/directus)

## Лицензия

MIT
