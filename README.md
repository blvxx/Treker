# Вдох / Vdoh

**Build better habits. Live better.**

«Вдох» — персональная платформа для формирования полезных привычек, отказа от вредных привычек и улучшения повседневного образа жизни. Долгосрочная концепция объединяет привычки, отказ от курения, дыхательные практики, тренировки, питание, AI-помощника и Telegram.

**Первый релиз:** private / personal use  
**Платформенная цель:** Web + Mobile + Telegram  
**Языки:** Русский и English

## Текущее состояние

Проект находится на этапе объединения и архитектурной подготовки.

Исходная реализация Treker — самостоятельный HTML/CSS/JavaScript прототип. Она уже включает:

- таймер с момента отказа от курения и временные этапы;
- ориентировочную статистику невыкуренных сигарет и экономии;
- журнал тяги с интенсивностью и заметками;
- дыхательные таймеры и визуализацию;
- локальное сохранение в браузере;
- экспорт данных в JSON;
- адаптивный интерфейс.

HabitForge пока содержит только README с концепцией трекера привычек. Его функции будут реализованы внутри единого приложения «Вдох»; отдельный готовый код HabitForge не переносится.

## Запуск текущего прототипа

Сборка и зависимости пока не нужны. Откройте `index.html` в современном браузере.

> Сейчас данные хранятся локально в браузере. Аккаунтов, backend и синхронизации между устройствами пока нет. Демонстрационные данные и информационные материалы требуют дальнейшей проверки.

## Целевая архитектура

- Web: Next.js + TypeScript
- Mobile: React Native + Expo
- Backend: Python + FastAPI
- Database: PostgreSQL
- Background jobs/cache: Redis
- AI: серверный AI gateway с ограниченными инструментами
- Telegram: bot integration
- QA: Pytest, Playwright, Maestro, GitHub Actions

Стек является целевым направлением, а не утверждением, что эти компоненты уже реализованы.

## Документация

- [Техническая ревизия](docs/TECHNICAL_AUDIT.md)
- [Продуктовые требования](docs/PRODUCT_SPEC.md)
- [Дорожная карта](docs/ROADMAP.md)
- [QA-стратегия](docs/QA_STRATEGY.md)

## Важное замечание

«Вдох» не является медицинским устройством, диагностическим сервисом или заменой консультации специалиста. AI-рекомендации и расчёты, связанные с питанием и физической активностью, должны иметь ограничения, проверяемые правила и подтверждение пользователя.

---

# English

**Vdoh** is a personal healthy-lifestyle platform concept focused on building sustainable habits and leaving harmful ones behind. The long-term product combines habit tracking, smoking cessation support, breathing exercises, workouts, nutrition, an integrated AI assistant, and Telegram.

The current codebase is an early Russian-language, browser-only prototype. The bilingual experience, backend, mobile app, AI features, and Telegram integration are planned and are not yet implemented.
