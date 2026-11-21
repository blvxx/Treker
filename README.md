# Вдох / Vdoh

**Build better habits. Live better.**

«Вдох» — мобильное приложение для формирования полезных привычек, отказа от вредных привычек и более осознанного образа жизни. Оно объединит привычки, поддержку отказа от курения, дыхательные практики, тренировки, питание и интегрированного AI-помощника.

**Основная платформа:** Android  
**Первый канал распространения:** Google Play  
**Первый релиз:** private testing / personal use  
**Языки:** Русский и English  
**Дополнительные интеграции:** Telegram; backend для синхронизации и AI

## Текущее состояние

Проект находится на этапе проектирования и подготовки мобильной архитектуры.

Исходный Treker — браузерный HTML/CSS/JavaScript прототип. Он уже содержит таймер отказа от курения, ориентировочную статистику, журнал тяги, дыхательные таймеры и визуализацию, локальное хранение и экспорт JSON.

HabitForge пока содержит только README с концепцией трекера привычек. Его идеи будут реализованы в мобильном приложении «Вдох»; готового кода для переноса нет.

Существующий Treker сохраняется как функциональный и визуальный reference. Его HTML/CSS не является основой Android UI: логику и полезные сценарии будем переносить в React Native, адаптируя интерфейс под мобильные паттерны.

## Целевая архитектура

- Android app: React Native + Expo + TypeScript
- Local storage: SQLite (через Expo SQLite) для локальных данных и offline-first сценариев
- Backend: Python + FastAPI
- Database: PostgreSQL
- Background jobs/cache: Redis — когда появится необходимость в серверных фоновых задачах
- AI: серверный AI gateway с ограниченными инструментами; секреты не хранятся в приложении
- Telegram: дополнительная интеграция для уведомлений и быстрых действий
- QA: Jest, React Native Testing Library, Pytest, Maestro, GitHub Actions

iOS может рассматриваться позднее благодаря React Native, но не входит в обязательный объём первого релиза. Отдельная веб-версия не является целью текущего этапа.

## Документация

- [Техническая ревизия](docs/TECHNICAL_AUDIT.md)
- [Продуктовые требования](docs/PRODUCT_SPEC.md)
- [Дорожная карта](docs/ROADMAP.md)
- [QA-стратегия](docs/QA_STRATEGY.md)

## Важное замечание

«Вдох» не является медицинским устройством, диагностическим сервисом или заменой консультации специалиста. AI-рекомендации и расчёты, связанные с питанием и физической активностью, должны иметь ограничения, проверяемые правила и подтверждение пользователя.

---

# English

**Vdoh** is an Android-first mobile app concept for building sustainable habits and leaving harmful ones behind. It will combine habit tracking, smoking cessation support, breathing exercises, workouts, nutrition, and an integrated AI assistant.

The first distribution target is Google Play, preceded by private testing. The current codebase is an early browser-only prototype; the native mobile app, backend, AI features, and Telegram integration are planned and are not yet implemented.
