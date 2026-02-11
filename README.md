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

## Рекомендації для подальшого ресерчу
- Порівняти production‑фічі: guardrails, tracing/observability, human‑in‑the‑loop, state persistence.
- Оцінити ecosystem: інтеграції, плагіни, MCP/конектори, деплой‑моделі.
- Виділити use‑cases: support‑боти, аналітика, RPA, dev assistants, ops automation.
