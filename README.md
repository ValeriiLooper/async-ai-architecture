# Async AI Architecture

**Модульная трехуровневая платформа для асинхронных AI-агентов**

---

## Русская версия

### Концепция
Модульная платформа для асинхронных AI-агентов с трехуровневой архитектурой управления.  

Система разделена на независимые контуры, чтобы **не перегружать LLM** и добиться минимальной задержки.

### 1. Трехуровневая архитектура управления
- **L1 (Fast Track)** — мгновенное реагирование по жёстким паттернам **без участия нейросети**.  
- **L2 (Orchestrator)** — логический планировщик, распределяет задачи и управляет состоянием сессии.  
- **L3 (Cognitive)** — используется **только** для сложных решений через локальную LLM.

### 2. Компонентная база (Planets)
Изолированные модули, работающие параллельно:
- **Data Node** — работа с базами данных, автоматическая генерация SQL.
- **Memory Node** — быстрое хранилище контекста с механизмом Recall.
- **Web Node** — высокоскоростное извлечение данных из интернета.

### 3. Стек
Python • Asyncio • LM Studio • Sqlite3

### 4. Ключевые преимущества
- Полная изоляция (сбой одного модуля не ломает систему)  
- Низкая задержка  
- Легко добавлять новые функции (новый Planet за одну итерацию)

### Для кого я делаю такие архитектуры
Я **не программист**, но отлично чувствую, как должна работать система.  
Моя сильная сторона — быстро переписывать эту архитектуру **под конкретную задачу или бизнес**.

Хотите:
- личного оффлайн-ассистента,
- агента-исследователя,
- корпоративного бота,
- систему мониторинга данных

— напишите мне, и я за 1–2 дня сделаю полностью адаптированную версию именно под вас.

**Контакты**  
Telegram: [@kovagen](https://t.me/kovagen)  
Email: valeriikormilets@gmail.com

---

## English version

### Concept
Modular three-level platform for asynchronous AI agents.

The system is divided into independent processing loops to **prevent LLM overload** and achieve low latency.

### 1. Three-level control architecture
- **L1 (Fast Track)** — instant deterministic responses using strict patterns **without any LLM**.  
- **L2 (Orchestrator)** — logical planner, distributes tasks and manages session state.  
- **L3 (Cognitive)** — used **only** for complex decisions via local LLM.

### 2. Component base (Planets)
Isolated functional blocks running in parallel threads:
- **Data Node** — autonomous database operations with automatic SQL generation.  
- **Memory Node** — fast context storage with Recall mechanism.  
- **Web Node** — high-speed web scraping and data extraction.

### 3. Tech stack
Python • Asyncio • LM Studio • Sqlite3

### 4. Key advantages
- Full isolation (one module failure doesn’t crash the system)  
- Low latency  
- Easy scalability (new Planet in one iteration)

### Who I build for
I’m **not a programmer**, but I have strong intuition for system design.  
My superpower is quickly rewriting this architecture for your specific needs.

Need a personal offline assistant, research agent, corporate bot or data monitoring system?  
Write to me — I’ll deliver a fully customized version in 1–2 days.

**Contacts**  
Telegram: [@kovagen](https://t.me/kovagen)  
Email: valeriikormilets@gmail.com

---

**Лицензия**  
Этот проект распространяется под лицензией Creative Commons Attribution 4.0 International (CC BY 4.0).  
Полный текст лицензии — в файле [LICENSE](LICENSE).
