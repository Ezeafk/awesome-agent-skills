# Awesome Agent Skills

> A curated list of reusable skills, workflows, and tool-backed capabilities for AI agents.

Languages: [English](README.md) | [简体中文](i18n/README.zh-CN.md) | [Português do Brasil](i18n/README.pt-BR.md) | [日本語](i18n/README.ja.md) | [Deutsch](i18n/README.de.md) | [Русский](i18n/README.ru.md)

This list focuses on reusable capabilities that help AI agents complete real tasks. It is not a prompt dump. A listed project should have a clear use case, reusable structure, installation or usage instructions, and enough context to explain inputs, outputs, and safety boundaries.

Last reviewed: 2026-07-18

## What Counts As A Skill

For this list, a skill is a reusable capability package for an AI agent. It may include instructions, workflows, scripts, references, templates, MCP servers, connectors, local app automation, validation steps, or examples.

## Legend

| Field | Values |
|---|---|
| Platform | Codex, Claude, ChatGPT, Cursor, Copilot, MCP, Generic Agent, n8n |
| Includes | Workflow, scripts, references, templates, MCP server, connector, app integration, examples |
| Status | Active = recent maintenance; Stable = still useful with slower updates; Use with care = valuable but sensitive |
| Risk | Low = mostly read-only or content generation; Medium = files, APIs, accounts, browser automation; High = production, security, deletion, payments, credentials, bulk actions |

## Evaluation Method

Skills are scored before inclusion. Stars are a weak signal only; a niche skill can be included when it solves a real task, has reusable structure, and gives agents enough instructions or tools to run safely.

| Area | Points | What reviewers check |
|---|---:|---|
| Task clarity | 0-2 | Clear real-world use case, inputs, outputs, and target user. |
| Reusable structure | 0-2 | More than a prompt: skill files, workflows, templates, scripts, examples, or references. |
| Platform and tool fit | 0-2 | Clear support for Codex, Claude, ChatGPT, Cursor, Copilot, MCP, n8n, CLI, browser, API, or local app workflows. |
| Validation and examples | 0-2 | Demo, tests, sample usage, CI checks, schema, or step-by-step verification. |
| Maintenance and safety | 0-2 | Recent activity, license clarity, safe defaults, confirmation rules, and credential/privacy guidance. |

Inclusion guide: 8-10 = recommended, 6-7 = acceptable with caveats, 4-5 = use with care or re-review, below 4 = remove or do not include. High-risk workflows need a stronger score and explicit safety notes.

## Contents

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
- [Evaluation Method](#evaluation-method)
- [Selection Criteria](#selection-criteria)

## Core Skill Registries

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [anthropics/skills](https://github.com/anthropics/skills) | Claude, Generic Agent | Public repository for Agent Skills. | Skills, examples, references | Active | Low |
| [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Claude Code, MCP, Generic Agent | Official Anthropic-managed directory of Claude Code plugins. | Plugins, skills, commands, agents, MCP configs | Active | Medium |
| [github/awesome-copilot](https://github.com/github/awesome-copilot) | Copilot, Generic Agent | Community instructions, agents, skills, and configurations. | Instructions, agents, skills, configs | Active | Low |
| [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) | Claude Code, Cursor, Copilot, Codex | Secure validated skill registry for professional coding agents. | Skill registry, validation, metadata | Active | Medium |
| [taishi-i/awesome-ChatGPT-repositories](https://github.com/taishi-i/awesome-ChatGPT-repositories) | ChatGPT, Codex, Claude | Searchable curated AI repository list exposed through Claude Code skills. | Awesome list, search workflow, skills | Active | Low |
| [JSONbored/awesome-claude](https://github.com/JSONbored/awesome-claude) | Claude, MCP, Generic Agent | Registry of Claude workflow assets, agents, MCP servers, skills, commands, and hooks. | Registry, agents, skills, MCP, commands | Active | Medium |
| [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Multi-role AI agency library with installable specialists for coding, security, content, product, and business workflows. | Agent library, install scripts, converters, examples | Active | Medium |
| [sickn33/agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) | Claude Code, Cursor, Codex, Gemini CLI | Large installable library of agentic skills for multiple coding agents. | Skill library, installer CLI, bundles, workflows | Active | Medium |
| [wshobson/agents](https://github.com/wshobson/agents) | Claude Code, Codex, Cursor, Copilot, Gemini CLI | Multi-harness agentic plugin marketplace for coding assistants. | Agents, workflows, plugins, MCP configs | Active | Medium |
| [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) | Generic Agent, Claude, Codex | Official Vercel collection of agent skills. | Skills, examples, workflows | Active | Medium |
| [farion1231/cc-switch](https://github.com/farion1231/cc-switch) | Claude Code, Codex, OpenCode, Gemini CLI | Desktop skills and provider manager for multiple coding agents. | Desktop app, skills management, provider switching | Active | Medium |
| [microsoft/SkillOpt](https://github.com/microsoft/SkillOpt) | Codex, Claude Code, Copilot, Cursor, Devin | Train, evaluate, and continuously improve reusable agent skills with trajectory-driven edits and held-out validation gates. | Skill optimizer, evals, benchmarks, plugins, WebUI | Active | High |

## Coding

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [openai/codex](https://github.com/openai/codex) | Codex | Terminal coding agent for repository tasks. | CLI, sandboxed workflows, code automation | Active | Medium |
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | Claude Code | Agentic coding in the terminal with repo context and git workflows. | CLI, tool workflows, coding automation | Active | Medium |
| [xai-org/grok-build](https://github.com/xai-org/grok-build) | Grok Build, Claude Code, Codex, MCP | Terminal coding agent with TUI, headless mode, skills, plugins, hooks, MCP, and sandboxing. | CLI, TUI, skills, plugins, MCP, hooks, sandbox | Active | Medium |
| [anthropics/claude-code-action](https://github.com/anthropics/claude-code-action) | Claude Code, GitHub | Run Claude Code workflows from GitHub Actions. | GitHub Action, automation workflow | Active | Medium |
| [jabrena/cursor-rules-java](https://github.com/jabrena/cursor-rules-java) | Cursor, Claude, Codex, Copilot | AI-native Java enterprise development workflow. | Rules, agents, commands, MCP servers | Active | Medium |
| [DollarDill/beads-superpowers](https://github.com/DollarDill/beads-superpowers) | Claude Code, Codex, OpenCode | Process-discipline skills and persistent task memory for coding agents. | Skills, task memory, TDD workflows | Active | Medium |
| [vosslab/vosslab-skills](https://github.com/vosslab/vosslab-skills) | Claude, Codex | Refactoring, code review, repo maintenance, and education content workflows. | Reusable skills, workflows | Active | Medium |
| [avalonreset/legends-github](https://github.com/avalonreset/legends-github) | Claude Code, Codex, Gemini CLI | GitHub repository optimization and community health workflows. | Skills, audit workflow, metadata checks | Active | Medium |
| [Jakevin/fastcontext-agent-tools](https://github.com/Jakevin/fastcontext-agent-tools) | Codex, MCP | Repository exploration with FastContext. | MCP server, Codex skill | Active | Medium |
| [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Claude Code, Codex, Cursor, Copilot | Production-grade engineering skills and lifecycle commands for AI coding agents. | Skills, commands, hooks, evals, references | Active | Medium |
| [alibaba/open-code-review](https://github.com/alibaba/open-code-review) | Claude Code, Codex, Cursor, OpenCode, MCP | Run precise diff or full-repository code reviews with deterministic file selection, agent context gathering, rules, and line-level findings. | CLI, skills, plugins, MCP, CI, rules, benchmarks | Active | High |
| [obra/superpowers](https://github.com/obra/superpowers) | Claude Code, Codex, Cursor, Copilot | Agentic software development methodology packaged as composable skills. | Skills framework, plugins, hooks, tests | Active | Medium |
| [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | Claude Code, Codex, Cursor, Gemini CLI | Turn codebases, schemas, docs, and media into a queryable knowledge graph for coding agents. | Knowledge graph, CLI, skills, tests | Active | Medium |
| [affaan-m/ECC](https://github.com/affaan-m/ECC) | Claude Code, Codex, Cursor, OpenCode | Harness optimization system with skills, memory, security, and research discipline. | Skills, memory, security workflows, MCP | Active | Medium |

## Data Analysis

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Kaelio/ktx](https://github.com/Kaelio/ktx) | Claude, Codex, MCP | Executable context layer for analytics agents. | Semantic context, database querying, MCP | Active | Medium |
| [dagster-io/dagster](https://github.com/dagster-io/dagster) | Generic Agent | Data asset orchestration for agent-driven analytics workflows. | Pipelines, schedules, observability | Active | Medium |
| [EtienneLescot/n8n-as-code](https://github.com/EtienneLescot/n8n-as-code) | n8n, Claude, Cursor, Copilot | Give agents n8n workflow creation and sync capabilities. | TypeScript workflows, schemas, templates | Active | Medium |
| [product-on-purpose/pm-skills](https://github.com/product-on-purpose/pm-skills) | Claude, Codex | Product management skill families and structured product workflows. | Skills, templates, examples, CI contracts | Active | Medium |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | Market research, strategy, and trading agent skills. | Awesome list, MCP servers, workflows | Active | High |

## Documents

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [yusufkaraaslan/Skill_Seekers](https://github.com/yusufkaraaslan/Skill_Seekers) | Claude | Convert docs, GitHub repos, and PDFs into Claude skills. | Parser, OCR, conflict detection, MCP | Active | Medium |
| [teng-lin/notebooklm-py](https://github.com/teng-lin/notebooklm-py) | Claude, Codex, Python | Programmatic NotebookLM workflows for agents. | Python API, CLI, agentic skill | Active | Medium |
| [chuspeeism/dashi-ppt-skill](https://github.com/chuspeeism/dashi-ppt-skill) | Claude Code, Codex, Cursor, Generic Agent | Generate browser-editable presentation decks with multiple themes and export them to HTML, PDF, and PPTX. | Skill, themes, templates, render scripts, exporters | Active | Medium |

## Design and Frontend

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [LingyiChen-AI/comfyui-workflow-skill](https://github.com/LingyiChen-AI/comfyui-workflow-skill) | Claude Code, Cursor, Generic Agent | Generate ComfyUI workflow JSON from natural language. | Templates, node definitions, model workflows | Active | Medium |
| [SlavaSexton/ComfyUI-Agent-Kit](https://github.com/SlavaSexton/ComfyUI-Agent-Kit) | Claude Code, Codex, Gemini CLI | Drive local ComfyUI end to end from an agent. | Skill, prompt recipes, templates, automation | Active | Medium |
| [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | Claude Code, Codex, Cursor, Copilot, Windsurf | End-to-end agentic video production from research and scripting through asset generation, editing, localization, rendering, and post-render QA. | 12 pipelines, 100+ tools, 700+ skills, schemas, Remotion, FFmpeg, tests | Active | High |
| [Orkas-AI/Orkas-VideoStudio](https://github.com/Orkas-AI/Orkas-VideoStudio) | Claude Code, Codex, Cursor, Generic Agent, MCP | Compose, edit, generate, transcribe, and assemble videos from editable timelines. | 14 skills, CLI, MCP server, `plan.json` schema, delivery guard, tests | Active | High |

## Browser and Web

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | MCP | Browser automation through Playwright MCP. | MCP server, browser tools | Active | Medium |
| [executeautomation/mcp-playwright](https://github.com/executeautomation/mcp-playwright) | MCP, Claude, Cursor | Browser and API automation through Playwright. | MCP server, Playwright workflows | Active | Medium |
| [browserbase/mcp-server-browserbase](https://github.com/browserbase/mcp-server-browserbase) | MCP | Let agents control cloud browsers with Browserbase and Stagehand. | MCP server, browser control | Active | Medium |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | OSINT tool discovery for research agents. | Curated MCP server list | Active | High |

## Security Skills

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | Claude, Codex, Generic Agent | Scan AI agent skills for malicious patterns, unsafe instructions, and security risks before installation. | Security scanner, CLI, reports, examples | Active | High |
| [cisco-ai-defense/skill-scanner](https://github.com/cisco-ai-defense/skill-scanner) | Claude, Generic Agent | Vet Agent Skills for supply-chain and prompt-level risks before teams adopt them. | Security scanner, rules, reports | Active | High |
| [snyk/agent-scan](https://github.com/snyk/agent-scan) | MCP, Generic Agent, Claude, Codex | Scan AI agents, MCP servers, and agent skills for vulnerabilities and risky tool behavior. | Security scanner, CLI, rules | Active | High |
| [trailofbits/skills](https://github.com/trailofbits/skills) | Claude Code | Security research, vulnerability detection, and audit workflows from Trail of Bits. | Skills, audit workflows, examples | Active | High |
| [Tencent/AI-Infra-Guard](https://github.com/Tencent/AI-Infra-Guard) | Generic Agent, MCP | Red-team AI infrastructure with agent, skill, MCP, jailbreak, and LLM security scans. | Red-team platform, scanners, reports | Active | High |

## DevOps and Cloud

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [rohitg00/awesome-devops-mcp-servers](https://github.com/rohitg00/awesome-devops-mcp-servers) | MCP, DevOps | DevOps-focused MCP servers and capabilities. | Curated MCP list, ops tools | Active | High |
| [Azure/awesome-azd](https://github.com/Azure/awesome-azd) | Azure, Generic Agent | Azure Developer CLI templates and workflows. | Templates, docs, deployment examples | Active | Medium |
| [AmoyLab/Unla](https://github.com/AmoyLab/Unla) | MCP | Transform APIs and MCP servers into managed MCP capabilities. | Gateway, UI, Docker deployment | Active | Medium |
| [milisp/mcp-linker](https://github.com/milisp/mcp-linker) | MCP, Claude, Cursor | Sync MCP server configurations across clients. | MCP manager, config sync | Active | Medium |
| [hashgraph-online/hol-guard](https://github.com/hashgraph-online/hol-guard) | Codex, Claude Code, Cursor, MCP | Scan plugins, skills, and MCP servers before tools run. | Security scanner, CLI, policy checks | Active | High |

## Research

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [GPTomics/bioSkills](https://github.com/GPTomics/bioSkills) | Claude Code, Generic Agent | Bioinformatics workflows for coding agents. | SKILLS.md files, domain workflows | Active | Medium |
| [modelscope/Awesome-Vibe-Research](https://github.com/modelscope/Awesome-Vibe-Research) | Generic Agent | Research resources for vibe research and agentic research. | Awesome list, research workflows | Active | Low |
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | ChatGPT, OpenAI API, Generic Agent | Examples and guides that can be adapted into agent workflows. | Examples, notebooks, API workflows | Active | Low |
| [simonw/llm](https://github.com/simonw/llm) | Generic Agent, CLI | Command-line LLM workflows and plugin-backed research tasks. | CLI, plugins, templates | Active | Medium |
| [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | Claude Code, Codex | Recency research skill for grounded summaries across social and web sources. | Skill, web research workflow, source synthesis | Active | Medium |
| [Astro-Han/karpathy-llm-wiki](https://github.com/Astro-Han/karpathy-llm-wiki) | Claude Code, Codex, Cursor, Generic Agent | Build a durable LLM-maintained wiki that ingests immutable sources, answers with citations, and lints evidence and links. | Skill, scripts, references, examples, linting | Active | Medium |
| [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | Claude Code, Codex, Cursor, Generic Agent | Scientific skill library for biology, chemistry, medicine, and research agents. | Scientific skills, databases, workflows | Active | High |

## MCP and Tool Integration

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) | MCP | Reference MCP servers for tool-backed agent capabilities. | MCP servers, examples | Active | Medium |
| [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | MCP | Large curated collection of MCP servers. | Awesome list, categories | Active | Medium |
| [appcypher/awesome-mcp-servers](https://github.com/appcypher/awesome-mcp-servers) | MCP | Curated list of MCP servers and tool-use capabilities. | Awesome list, server links | Active | Medium |
| [jaw9c/awesome-remote-mcp-servers](https://github.com/jaw9c/awesome-remote-mcp-servers) | MCP | Remote MCP server discovery. | Awesome list, remote services | Active | Medium |
| [ai-boost/awesome-a2a](https://github.com/ai-boost/awesome-a2a) | A2A, MCP, Generic Agent | Agent2Agent tools, servers, clients, and integrations. | Awesome list, protocols, tooling | Active | Medium |

## Finance Skills

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Bookkeeper & Controller](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-bookkeeper-controller.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Daily bookkeeping, general ledger, month-end close, reconciliation, internal controls, audit prep, and GAAP compliance. | Agent skill, finance workflow, controls checklist | Active | High |
| [Financial Analyst](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-financial-analyst.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Financial modeling, forecasting, scenario analysis, valuation, budget versus actuals, and operating decision support. | Agent skill, modeling workflow, analysis templates | Active | High |
| [FP&A Analyst](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-fpa-analyst.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Annual budgeting, rolling forecasts, operating plans, department budgets, KPIs, and monthly business reviews. | Agent skill, planning workflow, KPI review | Active | High |
| [Investment Researcher](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-investment-researcher.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Investment research, due diligence, asset valuation, portfolio analysis, bull and bear cases, and investment memos. | Agent skill, research workflow, valuation templates | Active | High |
| [Tax Strategist](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-tax-strategist.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Tax planning, multi-jurisdiction compliance, transfer pricing, entity structuring, and tax memoranda. | Agent skill, tax workflow, memo templates | Active | High |

## Business Workflows

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [enescingoz/awesome-n8n-templates](https://github.com/enescingoz/awesome-n8n-templates) | n8n, Generic Agent | Large workflow template collection for AI agents and business automation. | Workflow templates, integrations | Active | Medium |
| [lucaswalter/n8n-ai-automations](https://github.com/lucaswalter/n8n-ai-automations) | n8n | AI automations and agent workflows for business tools. | n8n workflows, examples | Active | Medium |
| [googleworkspace/cli](https://github.com/googleworkspace/cli) | Claude Code, Codex, Copilot, Gemini CLI, Generic Agent | Operate Drive, Gmail, Calendar, Sheets, Docs, Chat, and other Workspace APIs with CLI-backed skills, personas, and multi-step recipes. | CLI, 40+ skills, personas, recipes, structured JSON | Active | High |
| [AgriciDaniel/claude-seo](https://github.com/AgriciDaniel/claude-seo) | Claude Code, MCP, SEO, GEO | Comprehensive Claude Code SEO skill suite for technical SEO, content quality, schema, GEO/AEO, local SEO, backlinks, e-commerce, international SEO, and reporting. | Skills, sub-agents, commands, MCP extensions, reports, tests | Active | High |
| [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | Claude Code, Codex | Marketing skills for CRO, copywriting, SEO, analytics, and growth. | Skills, marketing workflows | Active | Medium |

## Personal Productivity

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Benkapner/claude-code-basecamp](https://github.com/Benkapner/claude-code-basecamp) | Claude Code | Workspace setup with skills, commands, and hooks. | Skills, commands, hooks | Active | Medium |
| [Daaaaave/agentic-workspace-core](https://github.com/Daaaaave/agentic-workspace-core) | Claude Code, Codex | Repository-native memory, skills, and knowledge workflows. | Memory, AGENTS.md, skills, llms.txt | Active | Medium |
| [WoJiSama/skill-based-architecture](https://github.com/WoJiSama/skill-based-architecture) | Cursor, Claude Code, Codex, Gemini | Meta-skill that distills repo knowledge into reusable skills. | Meta-skill, project skill generation | Active | Medium |
| [mksglu/context-mode](https://github.com/mksglu/context-mode) | Claude Code, Codex, Cursor, MCP | Optimize agent context windows with tool-output sandboxing, session memory, MCP, and hooks. | MCP server, hooks, skills, memory, plugins | Active | Medium |

## Use With Care

These projects can be valuable, but they involve sensitive domains such as security, trading, OSINT, privileged accounts, or agent-to-agent orchestration. Review permissions, confirmation steps, logs, and safety boundaries before using them.

| Skill | Platform | Use case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [gadievron/raptor](https://github.com/gadievron/raptor) | Claude Code | Offensive and defensive security agent workflows. | Rules, sub-agents, skills, security tools | Use with care | High |
| [matank001/cursor-security-rules](https://github.com/matank001/cursor-security-rules) | Cursor | Security rules for AI-assisted development workflows. | Cursor rules, guardrails | Use with care | High |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | Trading agents, market research, and execution resources. | Awesome list, MCP servers, agent skills | Use with care | High |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | OSINT MCP servers and investigative tooling. | Awesome list, MCP resources | Use with care | High |

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

Pull requests are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a skill.

## License

MIT. See [LICENSE](LICENSE).
