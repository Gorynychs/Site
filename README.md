# 🚚 Freight Site v2.0 | Production Architecture

## 📊 Статус проекта
✅ **Этап 1: Инициализация** — завершено  
⏳ **Этап 2: Бэкенд-ядро + Очереди** — в ожидании  
📅 Планируемый релиз MVP: 30-45 дней от старта

## 📁 Структура проекта# project
freight-site/
├── frontend/ # Клиентская часть (HTML/CSS/JS)
├── backend/ # Серверная логика (Express, Workers, Cache)
├── shared/ # Общие DTO, константы, валидаторы
├── database/ # Миграции, сиды, мониторинг запросов
├── deploy/ # Конфиги Vercel, Render, Docker, CI/CD
├── scripts/ # Автоматизация: бэкапы, откаты, чек-листы
├── logs/ # Аудит, ошибки, доступ, воркеры
├── docs/ # API_SPEC, COMPLIANCE, RUNBOOK, CHANGELOG
├── mocks/ # Фейковые API-ответы для тестов фронта
└── monitoring/ # Конфиги Sentry, Uptime, алерты

## 🚀 Быстрый запуск
1. Убедитесь, что установлен `Node.js >= 18` и `npm`
2. `cp .env.example .env` (заполните DEV-секцию)
3. `npm install && cd backend && npm install`
4. `npm run dev` (запуск сервера + подготовка фронта)
5. Перейдите в `http://localhost:3000/api/v1/health`

## 📚 Документация
- [🏗 Архитектура](docs/ARCHITECTURE.md)
- [🔌 API Спецификация](docs/API_SPEC.md)
- [🛡 Compliance 152-ФЗ](docs/COMPLIANCE.md)
- [🚨 Incident Runbook](docs/INCIDENT_RUNBOOK.md)
- [📦 Гайд по деплою](docs/DEPLOY_GUIDE.md)

## 🤝 Контрибьюция
Проект разрабатывается поэтапно под управлением заказчика. Все изменения фиксируются в `docs/CHANGELOG.md`.