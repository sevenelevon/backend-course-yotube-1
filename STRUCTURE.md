Структура нашего проекта

myproject/
├── cmd/
│   ├── main.go          # Точка входа в приложение
│
├── internal/
│   ├── handlers/        # Контроллеры HTTP-запросов
│   │   ├── user.go
│   │   ├── order.go
│   │   ├── book.go
│   │   └── category.go
│   │
│   ├── models/          # Модели данных
│   │   ├── user.go
│   │   ├── order.go
│   │   ├── book.go
│   │   └── category.go
│   │
│   ├── repositories/    # Репозитории для работы с базой данных
│   │   ├── user_repository.go
│   │   ├── order_repository.go
│   │   ├── book_repository.go
│   │   └── category_repository.go
│   │
│   ├── services/        # Сервисы бизнес-логики
│   │   ├── user_service.go
│   │   ├── order_service.go
│   │   ├── book_service.go
│   │   └── category_service.go
│   │
│   ├── middleware/      # Middleware для обработки запросов
│   │   ├── auth.go
│   │   ├── logging.go
│   │   └── ...
│   │
│   ├── config/          # Настройки приложения
│   │   ├── config.go
│   │   ├── database.go
│   │   └── ...
│
├── pkg/                 # Пакеты, используемые в приложении
│   ├── utils/
│   │   ├── helpers.go
│   │   ├── ...
│   │
│   ├── ...
│
├── migrations/           # Скрипты миграций базы данных
│   ├── 001_create_users_table.sql
│   ├── 002_create_orders_table.sql
│   ├── 003_create_books_table.sql
│   ├── 004_create_categories_table.sql
│   └── ...
│
├── static/               # Статические ресурсы (CSS, JS, изображения)
│
├── templates/            # HTML шаблоны
│
├── tests/                # Тесты
│   ├── user_test.go
│   ├── order_test.go
│   ├── book_test.go
│   ├── category_test.go
│   └── ...
│
├── .gitignore            # Игнорируемые файлы для Git
├── go.mod                # Модуль Go
├── go.sum                # Сумма модуля Go
└── README.md             # Документация и описание проекта