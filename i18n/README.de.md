# Awesome Agent Skills

> Kuratierte Liste wiederverwendbarer Skills, Workflows und tool-gestützter Fähigkeiten für AI Agents.

Sprachen: [English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

Diese Liste konzentriert sich auf wiederverwendbare Fähigkeiten, mit denen AI Agents echte Aufgaben erledigen können. Sie ist kein prompt dump. Ein gelistetes Projekt sollte einen klaren Use Case, wiederverwendbare Struktur, Installations- oder Nutzungsanweisungen und genügend Kontext zu Inputs, Outputs und Sicherheitsgrenzen haben.

Zuletzt geprüft: 2026-06-26

## Was Als Skill Zählt

In dieser Liste ist ein Skill ein wiederverwendbares Fähigkeitspaket für einen AI Agent. Es kann instructions, workflows, scripts, references, templates, MCP servers, connectors, local app automation, validation steps oder examples enthalten.

## Legende

| Feld | Werte |
|---|---|
| Platform | Codex, Claude, ChatGPT, Cursor, Copilot, MCP, Generic Agent, n8n |
| Includes | Workflow, scripts, references, templates, MCP server, connector, app integration, examples |
| Status | Active = kürzlich gepflegt; Stable = weiterhin nützlich bei langsameren Updates; Use with care = wertvoll, aber sensibel |
| Risk | Low = meist read-only oder Content-Erzeugung; Medium = Dateien, APIs, Accounts, Browser-Automation; High = Produktion, Security, Löschung, Zahlungen, Credentials, Massenaktionen |

## Inhalt

- [Core Skill Registries](#core-skill-registries)
- [Coding](#coding)
- [Data Analysis](#data-analysis)
- [Documents](#documents)
- [Design and Frontend](#design-and-frontend)
- [Browser and Web](#browser-and-web)
- [DevOps and Cloud](#devops-and-cloud)
- [Research](#research)
- [MCP and Tool Integration](#mcp-and-tool-integration)
- [Business Workflows](#business-workflows)
- [Personal Productivity](#personal-productivity)
- [Use With Care](#use-with-care)
- [Selection Criteria](#selection-criteria)

## Core Skill Registries

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [anthropics/skills](https://github.com/anthropics/skills) | Claude, Generic Agent | Öffentliches Repository für Agent Skills. | Skills, examples, references | Active | Low |
| [github/awesome-copilot](https://github.com/github/awesome-copilot) | Copilot, Generic Agent | Community-Instructions, Agents, Skills und Konfigurationen. | Instructions, agents, skills, configs | Active | Low |
| [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) | Claude Code, Cursor, Copilot, Codex | Sichere validierte Skill Registry für professionelle Coding Agents. | Skill registry, validation, metadata | Active | Medium |
| [taishi-i/awesome-ChatGPT-repositories](https://github.com/taishi-i/awesome-ChatGPT-repositories) | ChatGPT, Codex, Claude | Durchsuchbare kuratierte KI-Repository-Liste, verfügbar über Claude Code skills. | Awesome list, search workflow, skills | Active | Low |
| [JSONbored/awesome-claude](https://github.com/JSONbored/awesome-claude) | Claude, MCP, Generic Agent | Registry für Claude Workflow Assets, Agents, MCP servers, Skills, Commands und Hooks. | Registry, agents, skills, MCP, commands | Active | Medium |
| [linny006/awesome-agent-skills](https://github.com/linny006/awesome-agent-skills) | Generic Agent | Automatisch aktualisierte Awesome List für AI Agent Skills. | Awesome list, ratings, automation | Active | Low |

## Coding

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [openai/codex](https://github.com/openai/codex) | Codex | Terminal Coding Agent für Repository-Aufgaben. | CLI, sandboxed workflows, code automation | Active | Medium |
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | Claude Code | Agentic Coding im Terminal mit Repository-Kontext und git workflows. | CLI, tool workflows, coding automation | Active | Medium |
| [anthropics/claude-code-action](https://github.com/anthropics/claude-code-action) | Claude Code, GitHub | Claude Code workflows aus GitHub Actions ausführen. | GitHub Action, automation workflow | Active | Medium |
| [jabrena/cursor-rules-java](https://github.com/jabrena/cursor-rules-java) | Cursor, Claude, Codex, Copilot | AI-native Java Enterprise Development Workflow. | Rules, agents, commands, MCP servers | Active | Medium |
| [DollarDill/beads-superpowers](https://github.com/DollarDill/beads-superpowers) | Claude Code, Codex, OpenCode | Process-discipline Skills und persistenter Task Memory für Coding Agents. | Skills, task memory, TDD workflows | Active | Medium |
| [vosslab/vosslab-skills](https://github.com/vosslab/vosslab-skills) | Claude, Codex | Workflows für Refactoring, Code Review, Repository Maintenance und Bildungsinhalte. | Reusable skills, workflows | Active | Medium |
| [avalonreset/legends-github](https://github.com/avalonreset/legends-github) | Claude Code, Codex, Gemini CLI | Workflows für GitHub Repository Optimization und Community Health. | Skills, audit workflow, metadata checks | Active | Medium |
| [Jakevin/fastcontext-agent-tools](https://github.com/Jakevin/fastcontext-agent-tools) | Codex, MCP | Repository Exploration mit FastContext. | MCP server, Codex skill | Active | Medium |

## Data Analysis

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Kaelio/ktx](https://github.com/Kaelio/ktx) | Claude, Codex, MCP | Ausführbare Context Layer für Analytics Agents. | Semantic context, database querying, MCP | Active | Medium |
| [dagster-io/dagster](https://github.com/dagster-io/dagster) | Generic Agent | Data Asset Orchestration für agent-driven Analytics Workflows. | Pipelines, schedules, observability | Active | Medium |
| [EtienneLescot/n8n-as-code](https://github.com/EtienneLescot/n8n-as-code) | n8n, Claude, Cursor, Copilot | Agents mit n8n Workflow Creation und Sync Capabilities ausstatten. | TypeScript workflows, schemas, templates | Active | Medium |
| [product-on-purpose/pm-skills](https://github.com/product-on-purpose/pm-skills) | Claude, Codex | Product Management Skill Families und strukturierte Product Workflows. | Skills, templates, examples, CI contracts | Active | Medium |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | Market Research, Strategy und Trading Agent Skills. | Awesome list, MCP servers, workflows | Active | High |

## Documents

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [yusufkaraaslan/Skill_Seekers](https://github.com/yusufkaraaslan/Skill_Seekers) | Claude | Docs, GitHub Repos und PDFs in Claude skills umwandeln. | Parser, OCR, conflict detection, MCP | Active | Medium |
| [teng-lin/notebooklm-py](https://github.com/teng-lin/notebooklm-py) | Claude, Codex, Python | Programmatic NotebookLM workflows für Agents. | Python API, CLI, agentic skill | Active | Medium |
| [wuhanichina/powerlit-power-systems-writing-skills](https://github.com/wuhanichina/powerlit-power-systems-writing-skills) | Codex | Power-system Paper Writing Skills aus einem lokalen Corpus. | Writing skills, domain corpus | Active | Low |
| [kashmirscien3399/skills](https://github.com/kashmirscien3399/skills) | Generic Agent | Literature Review Automation für arXiv und Citation Tracking. | Research skills, fetch/extract workflows | Active | Medium |
| [londey/claude-skill-verilog](https://github.com/londey/claude-skill-verilog) | Claude Code | Mit Verilog über einen Domain Skill arbeiten. | Skill instructions, hardware domain workflow | Active | Low |

## Design and Frontend

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [LingyiChen-AI/comfyui-workflow-skill](https://github.com/LingyiChen-AI/comfyui-workflow-skill) | Claude Code, Cursor, Generic Agent | ComfyUI workflow JSON aus natürlicher Sprache generieren. | Templates, node definitions, model workflows | Active | Medium |
| [SlavaSexton/ComfyUI-Agent-Kit](https://github.com/SlavaSexton/ComfyUI-Agent-Kit) | Claude Code, Codex, Gemini CLI | Lokales ComfyUI end-to-end von einem Agent steuern. | Skill, prompt recipes, templates, automation | Active | Medium |
| [martgueritainaccurate875/skills](https://github.com/martgueritainaccurate875/skills) | Cursor, Gemini CLI, Generic Agent | Frontend-, Full-stack-, Mobile- und Shader-Development Skills. | Skill definitions, development workflows | Active | Medium |
| [AlexPEClub/ai-coding-starter-kit](https://github.com/AlexPEClub/ai-coding-starter-kit) | Generic Agent | Next.js starter mit spezialisierten AI Development Agents. | Template, agents, development workflow | Active | Medium |

## Browser and Web

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | MCP | Browser Automation über Playwright MCP. | MCP server, browser tools | Active | Medium |
| [executeautomation/mcp-playwright](https://github.com/executeautomation/mcp-playwright) | MCP, Claude, Cursor | Browser- und API-Automation über Playwright. | MCP server, Playwright workflows | Active | Medium |
| [browserbase/mcp-server-browserbase](https://github.com/browserbase/mcp-server-browserbase) | MCP | Agents Cloud Browsers mit Browserbase und Stagehand steuern lassen. | MCP server, browser control | Active | Medium |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | OSINT Tool Discovery für Research Agents. | Curated MCP server list | Active | High |

## DevOps and Cloud

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [rohitg00/awesome-devops-mcp-servers](https://github.com/rohitg00/awesome-devops-mcp-servers) | MCP, DevOps | DevOps-fokussierte MCP servers und Capabilities. | Curated MCP list, ops tools | Active | High |
| [Azure/awesome-azd](https://github.com/Azure/awesome-azd) | Azure, Generic Agent | Azure Developer CLI Templates und Workflows. | Templates, docs, deployment examples | Active | Medium |
| [AmoyLab/Unla](https://github.com/AmoyLab/Unla) | MCP | APIs und MCP servers in managed MCP capabilities transformieren. | Gateway, UI, Docker deployment | Active | Medium |
| [milisp/mcp-linker](https://github.com/milisp/mcp-linker) | MCP, Claude, Cursor | MCP server configurations über mehrere Clients synchronisieren. | MCP manager, config sync | Active | Medium |
| [hashgraph-online/hol-guard](https://github.com/hashgraph-online/hol-guard) | Codex, Claude Code, Cursor, MCP | Plugins, Skills und MCP servers scannen, bevor Tools laufen. | Security scanner, CLI, policy checks | Active | High |

## Research

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [GPTomics/bioSkills](https://github.com/GPTomics/bioSkills) | Claude Code, Generic Agent | Bioinformatics workflows für Coding Agents. | SKILLS.md files, domain workflows | Active | Medium |
| [modelscope/Awesome-Vibe-Research](https://github.com/modelscope/Awesome-Vibe-Research) | Generic Agent | Research Resources für Vibe Research und Agentic Research. | Awesome list, research workflows | Active | Low |
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | ChatGPT, OpenAI API, Generic Agent | Examples und Guides, die in Agent Workflows übernommen werden können. | Examples, notebooks, API workflows | Active | Low |
| [simonw/llm](https://github.com/simonw/llm) | Generic Agent, CLI | Command-line LLM workflows und plugin-backed Research Tasks. | CLI, plugins, templates | Active | Medium |

## MCP and Tool Integration

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) | MCP | Reference MCP servers für tool-backed Agent Capabilities. | MCP servers, examples | Active | Medium |
| [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | MCP | Große kuratierte Sammlung von MCP servers. | Awesome list, categories | Active | Medium |
| [appcypher/awesome-mcp-servers](https://github.com/appcypher/awesome-mcp-servers) | MCP | Kuratierte Liste von MCP servers und tool-use capabilities. | Awesome list, server links | Active | Medium |
| [jaw9c/awesome-remote-mcp-servers](https://github.com/jaw9c/awesome-remote-mcp-servers) | MCP | Entdeckung von Remote MCP servers. | Awesome list, remote services | Active | Medium |
| [ai-boost/awesome-a2a](https://github.com/ai-boost/awesome-a2a) | A2A, MCP, Generic Agent | Agent2Agent Tools, Servers, Clients und Integrationen. | Awesome list, protocols, tooling | Active | Medium |
| [Francis-Zxp/AI-SkillHub](https://github.com/Francis-Zxp/AI-SkillHub) | Codex, Claude Code, Antigravity | Desktop Skill Manager zum Importieren und Deployen von Skills. | Desktop app, skill import/sync | Active | Medium |
| [sametcelikbicak/rolecraft](https://github.com/sametcelikbicak/rolecraft) | Claude Code, Cursor, OpenCode | Zero-dependency CLI zur Installation von Agent Skills aus beliebigen Quellen. | CLI, installer workflow | Active | Medium |

## Business Workflows

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [enescingoz/awesome-n8n-templates](https://github.com/enescingoz/awesome-n8n-templates) | n8n, Generic Agent | Große Workflow Template Collection für AI Agents und Business Automation. | Workflow templates, integrations | Active | Medium |
| [lucaswalter/n8n-ai-automations](https://github.com/lucaswalter/n8n-ai-automations) | n8n | AI Automations und Agent Workflows für Business Tools. | n8n workflows, examples | Active | Medium |
| [carta/plugins](https://github.com/carta/plugins) | Claude, Codex, Copilot, MCP | Public Plugins und Skills für Equity/Startup Workflows. | Plugins, MCP, skills | Active | High |
| [tale-project/tale](https://github.com/tale-project/tale) | OpenClaw, Claude Code, Codex, Cursor | Arbeit über mehrere AI Agents orchestrieren und delegieren. | Orchestrator, workflows, MCP | Active | Medium |

## Personal Productivity

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Benkapner/claude-code-basecamp](https://github.com/Benkapner/claude-code-basecamp) | Claude Code | Workspace setup mit Skills, Commands und Hooks. | Skills, commands, hooks | Active | Medium |
| [Daaaaave/agentic-workspace-core](https://github.com/Daaaaave/agentic-workspace-core) | Claude Code, Codex | Repository-native Memory, Skills und Knowledge Workflows. | Memory, AGENTS.md, skills, llms.txt | Active | Medium |
| [WoJiSama/skill-based-architecture](https://github.com/WoJiSama/skill-based-architecture) | Cursor, Claude Code, Codex, Gemini | Meta-skill, der Repo-Wissen in wiederverwendbare Skills destilliert. | Meta-skill, project skill generation | Active | Medium |
| [JularDepick/user-thoughts.SKILL](https://github.com/JularDepick/user-thoughts.SKILL) | Codex, Claude Code, OpenCode | User Input in persistente projektgebundene Idea Repositories organisieren. | Agent skill, memory workflow | Active | Medium |
| [shiquda/skills-sync](https://github.com/shiquda/skills-sync) | Codex, Claude Code, Cursor | Lokale AI Agent Skills synchronisieren, versionieren und veröffentlichen. | CLI, GitHub publishing workflow | Active | Medium |
| [bardaxx/skillbook](https://github.com/bardaxx/skillbook) | Codex, Claude, Cursor | Portable Playbooks für Coding Agents. | Markdown workflows, sharing model | Active | Low |

## Use With Care

These projects can be valuable, but they involve sensitive domains such as security, trading, OSINT, privileged accounts, or agent-to-agent orchestration. Review permissions, confirmation steps, logs, and safety boundaries before using them.

| Skill | Platform | Use Case | Includes | Status | Risk |
|---|---|---|---|---|---|
| [gadievron/raptor](https://github.com/gadievron/raptor) | Claude Code | Offensive und defensive Security Agent Workflows. | Rules, sub-agents, skills, security tools | Use with care | High |
| [matank001/cursor-security-rules](https://github.com/matank001/cursor-security-rules) | Cursor | Security Rules für AI-assisted Development Workflows. | Cursor rules, guardrails | Use with care | High |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | Trading Agents, Market Research und Execution Resources. | Awesome list, MCP servers, agent skills | Use with care | High |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | OSINT MCP servers und investigative tooling. | Awesome list, MCP resources | Use with care | High |

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
