# AI Agent Platforms — Research

## Фокус
Агентні платформи та їх розвиток: фреймворки для оркестрації агентів, long-running workflows, контролю, безпеки та продакшн‑деплою.

## Ключові тренди розвитку
- Перехід від демо‑агентів до production‑ready систем (observability, tracing, guardrails, HITL).
- Stateful/long‑running агенти: durable execution, відновлення після збоїв, сесії/пам’ять.
- Зближення workflow‑оркестрації та agentic‑підходів (flows/graphs + агенти).
- Стандартизація інструментів та інтеграцій (plugin ecosystems, MCP, конектори).

## Платформи / фреймворки

### OpenAI Agents SDK
- Опис: легкий фреймворк для multi‑agent workflows; еволюція Swarm у production‑ready SDK.
- Фокус: agents, handoffs, guardrails, sessions, tracing.
- Джерело: https://github.com/openai/openai-agents-python

### OpenAI Swarm (experimental)
- Опис: освітній/експериментальний фреймворк для легкого multi‑agent orchestration; замінений Agents SDK.
- Джерело: https://github.com/openai/swarm

### Microsoft AutoGen
- Опис: фреймворк для multi‑agent застосунків (AgentChat), підтримує автономні агенти та співпрацю людина‑агент.
- Статус: підтримується, але нові користувачі спрямовуються на Microsoft Agent Framework; AutoGen отримує баг‑фікси/патчі.
- Джерело: https://github.com/microsoft/autogen

### LangGraph (LangChain)
- Опис: low‑level оркестрація для stateful, long‑running агентів; durable execution, HITL, memory, продакшн деплой.
- Підходить для складних графів/процесів з контролем стану.
- Джерело: https://docs.langchain.com/oss/python/langgraph/overview

### CrewAI
- Опис: Python‑фреймворк для role‑playing агентів; Crews/Flows; є enterprise control plane (observability, scaling).
- Фокус: простота, швидкий старт, командна робота агентів.
- Джерело: https://github.com/crewAIInc/crewAI

### Semantic Kernel
- Опис: enterprise‑ready SDK для агентів і multi‑agent систем; модель‑агностичний, plugin ecosystem, multi‑language (.NET/Java/Python).
- Фокус: інтеграції, безпека, стабільні API, enterprise use‑cases.
- Джерело: https://github.com/microsoft/semantic-kernel

### AutoGPT Platform
- Опис: платформа для побудови та запуску continuous агентів; self‑host + cloud beta.
- Фокус: end‑to‑end платформа (UI + backend) для агентів.
- Джерело: https://github.com/Significant-Gravitas/AutoGPT

## Можливості / функції (узагальнено)
- Оркестрація агентів: handoffs/делегація, ролі, координація, графи/flows.
- Statefulness: сесії/пам’ять, durable execution, відновлення після збоїв.
- Human‑in‑the‑loop: затвердження кроків, ручні interrupt/override.
- Guardrails: валідація input/output, policy‑checks.
- Observability: tracing/логування, метрики, дебаг execution‑графів.
- Інтеграції: tools, MCP/конектори, plugins, external services.

## Приклади застосування
- Support‑боти 24/7 з escalation до людини.
- RPA/операційна автоматизація (збір даних, звіти, рутини).
- Dev‑assistant у команді (code review, генерація тестів, triage задач).
- Аналітика/дослідження (multi‑agent research, структуровані звіти).
- Бізнес‑процеси (approval flows, routing, оркестрація департаментів).

## Платформні можливості (факти з джерел)

### OpenAI Agents SDK
- Вбудований agent loop, handoffs, guardrails, sessions, tracing.
- MCP server tool calling, function tools з валідацією.
- Realtime/voice‑agents, HITL.
- Джерело: https://openai.github.io/openai-agents-python/

### CrewAI
- Agents + tools + memory + knowledge + structured outputs.
- Flows з керуванням станом та long‑running workflows.
- Guardrails + observability (enterprise‑орієнтовано).
- Джерело: https://docs.crewai.com

### AutoGen
- AgentChat (multi‑agent conversational apps).
- AutoGen Studio (no‑code prototyping).
- Core: event‑driven framework для scalable multi‑agent систем.
- Extensions, MCP інтеграції, runtime для distributed agents.
- Джерело: https://microsoft.github.io/autogen/stable/

### AutoGPT Platform (self‑host)
- End‑to‑end платформа (UI + backend) для continuous‑agents.
- Self‑host сценарій з Docker/Node stack.
- Джерело: https://agpt.co/docs/platform/getting-started/getting-started

## Рекомендації для подальшого ресерчу
- Порівняти production‑фічі: guardrails, tracing/observability, human‑in‑the‑loop, state persistence.
- Оцінити ecosystem: інтеграції, плагіни, MCP/конектори, деплой‑моделі.
- Виділити use‑cases: support‑боти, аналітика, RPA, dev assistants, ops automation.
