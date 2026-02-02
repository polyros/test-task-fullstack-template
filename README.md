# Fullstack Code Review Challenge

## Легенда

Вы присоединились к команде разработки платформы прогнозов (prediction markets). Junior-разработчик написал простое приложение для управления списком items. Код работает, но требует ревью перед деплоем.

## Как начать

### 1. Создайте свой репозиторий

Нажмите кнопку **"Use this template"** → **"Create a new repository"**

- Название: любое (например, `test-task-solution`)
- Видимость: можно сделать **Private** (рекомендуется)
- Нажмите "Create repository"

### 2. Склонируйте свой репозиторий

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```

### 3. Создайте ветку для решения

```bash
git checkout -b solution
```

## Задание

### 1. Code Review (REVIEW.md)

Проведите ревью кода в `backend/` и `frontend/`:
- Найдите минимум **8 проблем** (backend, frontend, интеграция)
- Опишите каждую проблему и её последствия
- Предложите решения

### 2. Исправление кода

- Исправьте все найденные проблемы
- Сохраните функциональность
- Код должен компилироваться без ошибок

### 3. Тесты

- Backend: минимум 2 теста (pytest)
- Frontend: минимум 1 тест (vitest)

## Запуск

```bash
docker-compose up --build
```

- Backend: http://localhost:8000
- Frontend: http://localhost:3000
- API документация: http://localhost:8000/docs

## Структура проекта

```
test-task-fullstack-template/
├── README.md
├── REVIEW.md           # Ваш code review
├── docker-compose.yml
├── backend/
│   ├── Dockerfile
│   ├── pyproject.toml
│   ├── app/
│   │   ├── main.py
│   │   └── api/
│   │       └── items.py
│   └── tests/          # Добавьте тесты
└── frontend/
    ├── Dockerfile
    ├── package.json
    ├── vite.config.ts
    ├── src/
    │   ├── main.tsx
    │   ├── App.tsx
    │   └── components/
    │       └── ItemList.tsx
    └── tests/          # Добавьте тесты
```

## Как сдать решение

1. Запакуйте папки `backend/`, `frontend/` и файл `REVIEW.md` в ZIP-архив
2. Отправьте архив боту в Telegram
3. Бот автоматически проверит ваше решение и пришлёт результат

Проверка включает: линтер, типы, тесты и AI Code Review.

## Ограничения

- **Время:** 3 часа с момента начала
- **Инструменты:** IDE, документация, Google, Stack Overflow

### ВАЖНО: Запрет на AI для Code Review

**REVIEW.md должен быть написан вами лично, без использования AI-ассистентов.**

Мы проверяем именно ваши навыки анализа кода. AI-сгенерированные ревью легко распознаются и приводят к автоматическому отклонению.

Для написания кода AI-инструменты допустимы, но будьте готовы объяснить решения.

## Критерии оценки

| Критерий | Вес |
|----------|-----|
| Качество code review | 40% |
| Корректность исправлений | 30% |
| Покрытие тестами | 20% |
| Чистота кода | 10% |

---

Удачи!
