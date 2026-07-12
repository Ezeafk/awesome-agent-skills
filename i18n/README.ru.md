# Awesome Agent Skills

> Подборка переиспользуемых skills, workflows и tool-backed capabilities для AI agents.

Языки: [English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

Этот список посвящен переиспользуемым возможностям, которые помогают AI agents выполнять реальные задачи. Это не prompt dump. У проекта должен быть понятный use case, переиспользуемая структура, инструкции по установке или использованию и достаточно контекста про inputs, outputs и safety boundaries.

Последняя проверка: 2026-07-12

## Что Считается Skill

В этом списке skill означает переиспользуемый пакет возможностей для AI agent. Он может включать instructions, workflows, scripts, references, templates, MCP servers, connectors, local app automation, validation steps или examples.

## Обозначения

| Поле | Значения |
|---|---|
| Platform | Codex, Claude, ChatGPT, Cursor, Copilot, MCP, Generic Agent, n8n |
| Includes | Workflow, scripts, references, templates, MCP server, connector, app integration, examples |
| Status | Active = недавняя поддержка; Stable = все еще полезно, но обновляется медленнее; Use with care = ценно, но чувствительно |
| Risk | Low = в основном read-only или генерация контента; Medium = файлы, APIs, accounts, browser automation; High = production, security, deletion, payments, credentials, bulk actions |

## Метод Оценки

Skills оцениваются перед включением. Stars — только слабый сигнал; нишевый skill можно включить, если он решает реальную задачу, имеет переиспользуемую структуру и дает agents достаточно instructions или tools для безопасного выполнения.

| Область | Баллы | Что проверяется |
|---|---:|---|
| Ясность задачи | 0-2 | Понятный реальный use case, inputs, outputs и целевой пользователь. |
| Переиспользуемая структура | 0-2 | Больше чем prompt: skill files, workflows, templates, scripts, examples или references. |
| Платформа и инструменты | 0-2 | Явная поддержка Codex, Claude, ChatGPT, Cursor, Copilot, MCP, n8n, CLI, browser, API или local app workflows. |
| Валидация и примеры | 0-2 | Demo, tests, sample usage, CI checks, schema или step-by-step verification. |
| Поддержка и безопасность | 0-2 | Недавняя activity, понятная license, безопасные defaults, confirmation rules и credential/privacy guidance. |

Ориентир включения: 8-10 = рекомендуется, 6-7 = допустимо с оговорками, 4-5 = use with care или повторная проверка, ниже 4 = удалить или не включать. High-risk workflows требуют более высокого балла и явных заметок по безопасности.

## Содержание

- [Core Skill Registries](#core-skill-registries)
- [Coding](#coding)
- [Data Analysis](#data-analysis)
- [Documents](#documents)
- [Design and Frontend](#design-and-frontend)
- [Browser and Web](#browser-and-web)
- [Security Skills](#security-skills)
- [DevOps and Cloud](#devops-and-cloud)
- [Research](#research)
- [MCP and Tool Integration](#mcp-and-tool-integration)
- [Finance Skills](#finance-skills)
- [Business Workflows](#business-workflows)
- [Personal Productivity](#personal-productivity)
- [Use With Care](#use-with-care)
- [Метод Оценки](#метод-оценки)
- [Selection Criteria](#selection-criteria)

## Core Skill Registries

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [anthropics/skills](https://github.com/anthropics/skills) | Claude, Generic Agent | Публичный репозиторий для Agent Skills. | Skills, examples, references | Active | Low |
| [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Claude Code, MCP, Generic Agent | Официальный каталог Claude Code plugins, поддерживаемый Anthropic. | Plugins, skills, commands, agents, MCP configs | Active | Medium |
| [github/awesome-copilot](https://github.com/github/awesome-copilot) | Copilot, Generic Agent | Community instructions, agents, skills и configurations. | Instructions, agents, skills, configs | Active | Low |
| [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) | Claude Code, Cursor, Copilot, Codex | Безопасный проверенный skill registry для профессиональных coding agents. | Skill registry, validation, metadata | Active | Medium |
| [taishi-i/awesome-ChatGPT-repositories](https://github.com/taishi-i/awesome-ChatGPT-repositories) | ChatGPT, Codex, Claude | Поисковый curated список AI-репозиториев, доступный через Claude Code skills. | Awesome list, search workflow, skills | Active | Low |
| [JSONbored/awesome-claude](https://github.com/JSONbored/awesome-claude) | Claude, MCP, Generic Agent | Registry для Claude workflow assets, agents, MCP servers, skills, commands и hooks. | Registry, agents, skills, MCP, commands | Active | Medium |
| [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Устанавливаемая много-ролевая AI agency библиотека со специалистами для кодинга, безопасности, контента, продукта и бизнес-процессов. | Agent library, install scripts, converters, examples | Active | Medium |
| [sickn33/agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) | Claude Code, Cursor, Codex, Gemini CLI | Большая installable library agentic skills для разных coding agents. | Skill library, installer CLI, bundles, workflows | Active | Medium |
| [wshobson/agents](https://github.com/wshobson/agents) | Claude Code, Codex, Cursor, Copilot, Gemini CLI | Multi-harness agentic plugin marketplace для coding assistants. | Agents, workflows, plugins, MCP configs | Active | Medium |
| [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) | Generic Agent, Claude, Codex | Официальная коллекция agent skills от Vercel. | Skills, examples, workflows | Active | Medium |
| [farion1231/cc-switch](https://github.com/farion1231/cc-switch) | Claude Code, Codex, OpenCode, Gemini CLI | Desktop skills и provider manager для нескольких coding agents. | Desktop app, skills management, provider switching | Active | Medium |

## Coding

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [openai/codex](https://github.com/openai/codex) | Codex | Terminal coding agent для задач с репозиториями. | CLI, sandboxed workflows, code automation | Active | Medium |
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | Claude Code | Agentic coding в терминале с контекстом репозитория и git workflows. | CLI, tool workflows, coding automation | Active | Medium |
| [anthropics/claude-code-action](https://github.com/anthropics/claude-code-action) | Claude Code, GitHub | Запуск Claude Code workflows из GitHub Actions. | GitHub Action, automation workflow | Active | Medium |
| [jabrena/cursor-rules-java](https://github.com/jabrena/cursor-rules-java) | Cursor, Claude, Codex, Copilot | AI-native workflow для Java enterprise development. | Rules, agents, commands, MCP servers | Active | Medium |
| [DollarDill/beads-superpowers](https://github.com/DollarDill/beads-superpowers) | Claude Code, Codex, OpenCode | Process-discipline skills и постоянная task memory для coding agents. | Skills, task memory, TDD workflows | Active | Medium |
| [vosslab/vosslab-skills](https://github.com/vosslab/vosslab-skills) | Claude, Codex | Workflows для refactoring, code review, repo maintenance и educational content. | Reusable skills, workflows | Active | Medium |
| [avalonreset/legends-github](https://github.com/avalonreset/legends-github) | Claude Code, Codex, Gemini CLI | Workflows для GitHub repository optimization и community health. | Skills, audit workflow, metadata checks | Active | Medium |
| [Jakevin/fastcontext-agent-tools](https://github.com/Jakevin/fastcontext-agent-tools) | Codex, MCP | Исследование репозиториев с FastContext. | MCP server, Codex skill | Active | Medium |
| [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Claude Code, Codex, Cursor, Copilot | Production-grade engineering skills и lifecycle commands для AI coding agents. | Skills, commands, hooks, evals, references | Active | Medium |
| [obra/superpowers](https://github.com/obra/superpowers) | Claude Code, Codex, Cursor, Copilot | Методология agentic software development, упакованная как комбинируемые skills. | Skills framework, plugins, hooks, tests | Active | Medium |
| [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | Claude Code, Codex, Cursor, Gemini CLI | Превращает codebases, schemas, docs и media в queryable knowledge graph для coding agents. | Knowledge graph, CLI, skills, tests | Active | Medium |
| [affaan-m/ECC](https://github.com/affaan-m/ECC) | Claude Code, Codex, Cursor, OpenCode | Harness optimization system со skills, memory, security и research discipline. | Skills, memory, security workflows, MCP | Active | Medium |

## Data Analysis

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Kaelio/ktx](https://github.com/Kaelio/ktx) | Claude, Codex, MCP | Executable context layer для analytics agents. | Semantic context, database querying, MCP | Active | Medium |
| [dagster-io/dagster](https://github.com/dagster-io/dagster) | Generic Agent | Data asset orchestration для agent-driven analytics workflows. | Pipelines, schedules, observability | Active | Medium |
| [EtienneLescot/n8n-as-code](https://github.com/EtienneLescot/n8n-as-code) | n8n, Claude, Cursor, Copilot | Дает agents возможности создания и синхронизации n8n workflows. | TypeScript workflows, schemas, templates | Active | Medium |
| [product-on-purpose/pm-skills](https://github.com/product-on-purpose/pm-skills) | Claude, Codex | Product management skill families и структурированные product workflows. | Skills, templates, examples, CI contracts | Active | Medium |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | Market research, strategy и trading agent skills. | Awesome list, MCP servers, workflows | Active | High |

## Documents

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [yusufkaraaslan/Skill_Seekers](https://github.com/yusufkaraaslan/Skill_Seekers) | Claude | Преобразование docs, GitHub repos и PDFs в Claude skills. | Parser, OCR, conflict detection, MCP | Active | Medium |
| [teng-lin/notebooklm-py](https://github.com/teng-lin/notebooklm-py) | Claude, Codex, Python | Programmatic NotebookLM workflows для agents. | Python API, CLI, agentic skill | Active | Medium |

## Design and Frontend

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [LingyiChen-AI/comfyui-workflow-skill](https://github.com/LingyiChen-AI/comfyui-workflow-skill) | Claude Code, Cursor, Generic Agent | Генерация ComfyUI workflow JSON из естественного языка. | Templates, node definitions, model workflows | Active | Medium |
| [SlavaSexton/ComfyUI-Agent-Kit](https://github.com/SlavaSexton/ComfyUI-Agent-Kit) | Claude Code, Codex, Gemini CLI | Управление локальным ComfyUI end to end из agent. | Skill, prompt recipes, templates, automation | Active | Medium |

## Browser and Web

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | MCP | Browser automation через Playwright MCP. | MCP server, browser tools | Active | Medium |
| [executeautomation/mcp-playwright](https://github.com/executeautomation/mcp-playwright) | MCP, Claude, Cursor | Browser и API automation через Playwright. | MCP server, Playwright workflows | Active | Medium |
| [browserbase/mcp-server-browserbase](https://github.com/browserbase/mcp-server-browserbase) | MCP | Позволяет agents управлять cloud browsers через Browserbase и Stagehand. | MCP server, browser control | Active | Medium |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | OSINT tool discovery для research agents. | Curated MCP server list | Active | High |

## Security Skills

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | Claude, Codex, Generic Agent | Сканировать AI agent skills перед установкой на вредоносные паттерны, небезопасные инструкции и риски безопасности. | Security scanner, CLI, reports, examples | Active | High |
| [cisco-ai-defense/skill-scanner](https://github.com/cisco-ai-defense/skill-scanner) | Claude, Generic Agent | Проверять Agent Skills перед внедрением в команде на риски supply chain и prompt-уровня. | Security scanner, rules, reports | Active | High |
| [snyk/agent-scan](https://github.com/snyk/agent-scan) | MCP, Generic Agent, Claude, Codex | Сканировать AI agents, MCP servers и agent skills на уязвимости и рискованное поведение tools. | Security scanner, CLI, rules | Active | High |
| [trailofbits/skills](https://github.com/trailofbits/skills) | Claude Code | Workflows от Trail of Bits для security research, поиска уязвимостей и аудита. | Skills, audit workflows, examples | Active | High |
| [Tencent/AI-Infra-Guard](https://github.com/Tencent/AI-Infra-Guard) | Generic Agent, MCP | Проводить red-team проверку AI-инфраструктуры через сканы agent, skill, MCP, jailbreak и LLM security. | Red-team platform, scanners, reports | Active | High |

## DevOps and Cloud

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [rohitg00/awesome-devops-mcp-servers](https://github.com/rohitg00/awesome-devops-mcp-servers) | MCP, DevOps | DevOps-focused MCP servers и capabilities. | Curated MCP list, ops tools | Active | High |
| [Azure/awesome-azd](https://github.com/Azure/awesome-azd) | Azure, Generic Agent | Azure Developer CLI templates и workflows. | Templates, docs, deployment examples | Active | Medium |
| [AmoyLab/Unla](https://github.com/AmoyLab/Unla) | MCP | Преобразование APIs и MCP servers в managed MCP capabilities. | Gateway, UI, Docker deployment | Active | Medium |
| [milisp/mcp-linker](https://github.com/milisp/mcp-linker) | MCP, Claude, Cursor | Синхронизация MCP server configurations между clients. | MCP manager, config sync | Active | Medium |
| [hashgraph-online/hol-guard](https://github.com/hashgraph-online/hol-guard) | Codex, Claude Code, Cursor, MCP | Сканирование plugins, skills и MCP servers перед запуском tools. | Security scanner, CLI, policy checks | Active | High |

## Research

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [GPTomics/bioSkills](https://github.com/GPTomics/bioSkills) | Claude Code, Generic Agent | Bioinformatics workflows для coding agents. | SKILLS.md files, domain workflows | Active | Medium |
| [modelscope/Awesome-Vibe-Research](https://github.com/modelscope/Awesome-Vibe-Research) | Generic Agent | Research resources для vibe research и agentic research. | Awesome list, research workflows | Active | Low |
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | ChatGPT, OpenAI API, Generic Agent | Examples и guides, которые можно адаптировать в agent workflows. | Examples, notebooks, API workflows | Active | Low |
| [simonw/llm](https://github.com/simonw/llm) | Generic Agent, CLI | Command-line LLM workflows и plugin-backed research tasks. | CLI, plugins, templates | Active | Medium |
| [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | Claude Code, Codex | Research skill для grounded summaries по свежим social и web sources. | Skill, web research workflow, source synthesis | Active | Medium |
| [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | Claude Code, Codex, Cursor, Generic Agent | Библиотека scientific skills для biology, chemistry, medicine и research agents. | Scientific skills, databases, workflows | Active | High |

## MCP and Tool Integration

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) | MCP | Reference MCP servers для tool-backed agent capabilities. | MCP servers, examples | Active | Medium |
| [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | MCP | Большая curated collection MCP servers. | Awesome list, categories | Active | Medium |
| [appcypher/awesome-mcp-servers](https://github.com/appcypher/awesome-mcp-servers) | MCP | Curated list MCP servers и tool-use capabilities. | Awesome list, server links | Active | Medium |
| [jaw9c/awesome-remote-mcp-servers](https://github.com/jaw9c/awesome-remote-mcp-servers) | MCP | Обнаружение remote MCP servers. | Awesome list, remote services | Active | Medium |
| [ai-boost/awesome-a2a](https://github.com/ai-boost/awesome-a2a) | A2A, MCP, Generic Agent | Agent2Agent tools, servers, clients и integrations. | Awesome list, protocols, tooling | Active | Medium |

## Finance Skills

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Bookkeeper & Controller](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-bookkeeper-controller.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Ежедневный учет, главная книга, месячное закрытие, сверки, внутренний контроль, подготовка к аудиту и соответствие GAAP. | Agent skill, finance workflow, controls checklist | Active | High |
| [Financial Analyst](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-financial-analyst.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Финансовое моделирование, прогнозирование, сценарный анализ, оценка, анализ бюджет-факт и поддержка операционных решений. | Agent skill, modeling workflow, analysis templates | Active | High |
| [FP&A Analyst](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-fpa-analyst.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Годовой бюджет, скользящие прогнозы, операционные планы, бюджеты подразделений, KPI и ежемесячные бизнес-обзоры. | Agent skill, planning workflow, KPI review | Active | High |
| [Investment Researcher](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-investment-researcher.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Инвестиционное исследование, due diligence, оценка активов, анализ портфеля, bull/bear сценарии и инвестиционные меморандумы. | Agent skill, research workflow, valuation templates | Active | High |
| [Tax Strategist](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-tax-strategist.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Налоговое планирование, compliance в разных юрисдикциях, трансфертное ценообразование, структура юрлиц и налоговые меморандумы. | Agent skill, tax workflow, memo templates | Active | High |

## Business Workflows

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [enescingoz/awesome-n8n-templates](https://github.com/enescingoz/awesome-n8n-templates) | n8n, Generic Agent | Большая коллекция workflow templates для AI agents и business automation. | Workflow templates, integrations | Active | Medium |
| [lucaswalter/n8n-ai-automations](https://github.com/lucaswalter/n8n-ai-automations) | n8n | AI automations и agent workflows для business tools. | n8n workflows, examples | Active | Medium |
| [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | Claude Code, Codex | Marketing skills для CRO, copywriting, SEO, analytics и growth. | Skills, marketing workflows | Active | Medium |

## Personal Productivity

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Benkapner/claude-code-basecamp](https://github.com/Benkapner/claude-code-basecamp) | Claude Code | Workspace setup со skills, commands и hooks. | Skills, commands, hooks | Active | Medium |
| [Daaaaave/agentic-workspace-core](https://github.com/Daaaaave/agentic-workspace-core) | Claude Code, Codex | Repository-native memory, skills и knowledge workflows. | Memory, AGENTS.md, skills, llms.txt | Active | Medium |
| [WoJiSama/skill-based-architecture](https://github.com/WoJiSama/skill-based-architecture) | Cursor, Claude Code, Codex, Gemini | Meta-skill, который превращает знания repo в reusable skills. | Meta-skill, project skill generation | Active | Medium |
| [mksglu/context-mode](https://github.com/mksglu/context-mode) | Claude Code, Codex, Cursor, MCP | Оптимизирует context windows агентов через sandboxing tool output, session memory, MCP и hooks. | MCP server, hooks, skills, memory, plugins | Active | Medium |

## Use With Care

These projects can be valuable, but they involve sensitive domains such as security, trading, OSINT, privileged accounts, or agent-to-agent orchestration. Review permissions, confirmation steps, logs, and safety boundaries before using them.

| Skill | Platform | Сценарий | Includes | Status | Risk |
|---|---|---|---|---|---|
| [gadievron/raptor](https://github.com/gadievron/raptor) | Claude Code | Offensive и defensive security agent workflows. | Rules, sub-agents, skills, security tools | Use with care | High |
| [matank001/cursor-security-rules](https://github.com/matank001/cursor-security-rules) | Cursor | Security rules для AI-assisted development workflows. | Cursor rules, guardrails | Use with care | High |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | Trading agents, market research и execution resources. | Awesome list, MCP servers, agent skills | Use with care | High |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | OSINT MCP servers и investigative tooling. | Awesome list, MCP resources | Use with care | High |

## Selection Criteria

### Must Have

- A clear task-oriented use case.
- Reusable structure beyond a single prompt.
- Installation, copy, or usage instructions.
- A stated platform or runtime environment.
- Inputs and outputs that can be understood by a new user.

### Preferred

- Real examples or demos.
- Validation steps or tests.
- Safety boundaries and confirmation rules.
- Scripts, references, templates, MCP servers, connectors, or tool docs.
- Complete task workflows rather than isolated instructions.

### Not Included

- Prompt dumps.
- One-line role presets.
- Unstructured system prompts without examples.
- Marketing-only agent templates.
- High-risk automation without confirmation mechanisms.
- Projects asking for sensitive credentials without privacy or security guidance.

## Contributing

Pull requests are welcome. Please read [CONTRIBUTING.md](../CONTRIBUTING.md) before submitting a skill.

## License

MIT. See [LICENSE](../LICENSE).
