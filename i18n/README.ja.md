# Awesome Agent Skills

> AI agents 向けの再利用可能な skills、workflows、tool-backed capabilities の厳選リスト。

言語: [English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

このリストは、AI agents が実際のタスクを完了するための再利用可能な能力に焦点を当てています。prompt dump ではありません。掲載プロジェクトには明確なユースケース、再利用可能な構造、インストールまたは利用手順、入力・出力・安全境界を説明できる情報が必要です。

最終確認日: 2026-06-26

## Skill の定義

このリストでは、skill は AI agent のための再利用可能な能力パッケージです。instructions、workflows、scripts、references、templates、MCP servers、connectors、local app automation、validation steps、examples などを含みます。

## 凡例

| 項目 | 値 |
|---|---|
| Platform | Codex, Claude, ChatGPT, Cursor, Copilot, MCP, Generic Agent, n8n |
| Includes | Workflow, scripts, references, templates, MCP server, connector, app integration, examples |
| Status | Active = 最近メンテナンスあり；Stable = 更新は遅いが有用；Use with care = 有用だが慎重な扱いが必要 |
| Risk | Low = 主に読み取りまたはコンテンツ生成；Medium = files、APIs、accounts、browser automation；High = production、security、deletion、payments、credentials、bulk actions |

## 目次

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

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [anthropics/skills](https://github.com/anthropics/skills) | Claude, Generic Agent | Agent Skills の公開リポジトリ。 | Skills, examples, references | Active | Low |
| [github/awesome-copilot](https://github.com/github/awesome-copilot) | Copilot, Generic Agent | コミュニティによる instructions、agents、skills、configurations。 | Instructions, agents, skills, configs | Active | Low |
| [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) | Claude Code, Cursor, Copilot, Codex | プロ向け coding agents のための安全に検証された skill registry。 | Skill registry, validation, metadata | Active | Medium |
| [taishi-i/awesome-ChatGPT-repositories](https://github.com/taishi-i/awesome-ChatGPT-repositories) | ChatGPT, Codex, Claude | Claude Code skills から利用できる検索可能な AI リポジトリ厳選リスト。 | Awesome list, search workflow, skills | Active | Low |
| [JSONbored/awesome-claude](https://github.com/JSONbored/awesome-claude) | Claude, MCP, Generic Agent | Claude workflow assets、agents、MCP servers、skills、commands、hooks の registry。 | Registry, agents, skills, MCP, commands | Active | Medium |
| [linny006/awesome-agent-skills](https://github.com/linny006/awesome-agent-skills) | Generic Agent | 自動更新される AI agent skills の awesome list。 | Awesome list, ratings, automation | Active | Low |

## Coding

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [openai/codex](https://github.com/openai/codex) | Codex | リポジトリ作業向けのターミナル coding agent。 | CLI, sandboxed workflows, code automation | Active | Medium |
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | Claude Code | リポジトリコンテキストと git workflows を使うターミナルでの agentic coding。 | CLI, tool workflows, coding automation | Active | Medium |
| [anthropics/claude-code-action](https://github.com/anthropics/claude-code-action) | Claude Code, GitHub | GitHub Actions から Claude Code workflows を実行。 | GitHub Action, automation workflow | Active | Medium |
| [jabrena/cursor-rules-java](https://github.com/jabrena/cursor-rules-java) | Cursor, Claude, Codex, Copilot | AI-native な Java enterprise development workflow。 | Rules, agents, commands, MCP servers | Active | Medium |
| [DollarDill/beads-superpowers](https://github.com/DollarDill/beads-superpowers) | Claude Code, Codex, OpenCode | coding agents 向けの process-discipline skills と永続的な task memory。 | Skills, task memory, TDD workflows | Active | Medium |
| [vosslab/vosslab-skills](https://github.com/vosslab/vosslab-skills) | Claude, Codex | リファクタリング、code review、repo maintenance、教育コンテンツ制作の workflows。 | Reusable skills, workflows | Active | Medium |
| [avalonreset/legends-github](https://github.com/avalonreset/legends-github) | Claude Code, Codex, Gemini CLI | GitHub repository optimization と community health の workflows。 | Skills, audit workflow, metadata checks | Active | Medium |
| [Jakevin/fastcontext-agent-tools](https://github.com/Jakevin/fastcontext-agent-tools) | Codex, MCP | FastContext による repository exploration。 | MCP server, Codex skill | Active | Medium |

## Data Analysis

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Kaelio/ktx](https://github.com/Kaelio/ktx) | Claude, Codex, MCP | analytics agents 向けの executable context layer。 | Semantic context, database querying, MCP | Active | Medium |
| [dagster-io/dagster](https://github.com/dagster-io/dagster) | Generic Agent | agent-driven analytics workflows のための data asset orchestration。 | Pipelines, schedules, observability | Active | Medium |
| [EtienneLescot/n8n-as-code](https://github.com/EtienneLescot/n8n-as-code) | n8n, Claude, Cursor, Copilot | agents に n8n workflow の作成と同期能力を与える。 | TypeScript workflows, schemas, templates | Active | Medium |
| [product-on-purpose/pm-skills](https://github.com/product-on-purpose/pm-skills) | Claude, Codex | product management skill families と構造化された product workflows。 | Skills, templates, examples, CI contracts | Active | Medium |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | 市場調査、戦略、trading agent skills。 | Awesome list, MCP servers, workflows | Active | High |

## Documents

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [yusufkaraaslan/Skill_Seekers](https://github.com/yusufkaraaslan/Skill_Seekers) | Claude | docs、GitHub repos、PDFs を Claude skills に変換。 | Parser, OCR, conflict detection, MCP | Active | Medium |
| [teng-lin/notebooklm-py](https://github.com/teng-lin/notebooklm-py) | Claude, Codex, Python | agents 向けの NotebookLM programmatic workflows。 | Python API, CLI, agentic skill | Active | Medium |
| [wuhanichina/powerlit-power-systems-writing-skills](https://github.com/wuhanichina/powerlit-power-systems-writing-skills) | Codex | ローカル corpus から作る power-system paper writing skills。 | Writing skills, domain corpus | Active | Low |
| [kashmirscien3399/skills](https://github.com/kashmirscien3399/skills) | Generic Agent | arXiv と citation tracking の literature review automation。 | Research skills, fetch/extract workflows | Active | Medium |
| [londey/claude-skill-verilog](https://github.com/londey/claude-skill-verilog) | Claude Code | ドメイン skill を使って Verilog を扱う。 | Skill instructions, hardware domain workflow | Active | Low |

## Design and Frontend

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [LingyiChen-AI/comfyui-workflow-skill](https://github.com/LingyiChen-AI/comfyui-workflow-skill) | Claude Code, Cursor, Generic Agent | 自然言語から ComfyUI workflow JSON を生成。 | Templates, node definitions, model workflows | Active | Medium |
| [SlavaSexton/ComfyUI-Agent-Kit](https://github.com/SlavaSexton/ComfyUI-Agent-Kit) | Claude Code, Codex, Gemini CLI | agent からローカル ComfyUI をエンドツーエンドで操作。 | Skill, prompt recipes, templates, automation | Active | Medium |
| [martgueritainaccurate875/skills](https://github.com/martgueritainaccurate875/skills) | Cursor, Gemini CLI, Generic Agent | frontend、full-stack、mobile、shader development skills。 | Skill definitions, development workflows | Active | Medium |
| [AlexPEClub/ai-coding-starter-kit](https://github.com/AlexPEClub/ai-coding-starter-kit) | Generic Agent | 専門 AI development agents を備えた Next.js starter。 | Template, agents, development workflow | Active | Medium |

## Browser and Web

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | MCP | Playwright MCP による browser automation。 | MCP server, browser tools | Active | Medium |
| [executeautomation/mcp-playwright](https://github.com/executeautomation/mcp-playwright) | MCP, Claude, Cursor | Playwright による browser と API automation。 | MCP server, Playwright workflows | Active | Medium |
| [browserbase/mcp-server-browserbase](https://github.com/browserbase/mcp-server-browserbase) | MCP | Browserbase と Stagehand で agents が cloud browsers を制御できるようにする。 | MCP server, browser control | Active | Medium |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | research agents 向けの OSINT tool discovery。 | Curated MCP server list | Active | High |

## DevOps and Cloud

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [rohitg00/awesome-devops-mcp-servers](https://github.com/rohitg00/awesome-devops-mcp-servers) | MCP, DevOps | DevOps に特化した MCP servers と capabilities。 | Curated MCP list, ops tools | Active | High |
| [Azure/awesome-azd](https://github.com/Azure/awesome-azd) | Azure, Generic Agent | Azure Developer CLI templates と workflows。 | Templates, docs, deployment examples | Active | Medium |
| [AmoyLab/Unla](https://github.com/AmoyLab/Unla) | MCP | APIs と MCP servers を managed MCP capabilities に変換。 | Gateway, UI, Docker deployment | Active | Medium |
| [milisp/mcp-linker](https://github.com/milisp/mcp-linker) | MCP, Claude, Cursor | 複数 clients 間で MCP server configurations を同期。 | MCP manager, config sync | Active | Medium |
| [hashgraph-online/hol-guard](https://github.com/hashgraph-online/hol-guard) | Codex, Claude Code, Cursor, MCP | tools 実行前に plugins、skills、MCP servers をスキャン。 | Security scanner, CLI, policy checks | Active | High |

## Research

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [GPTomics/bioSkills](https://github.com/GPTomics/bioSkills) | Claude Code, Generic Agent | coding agents 向けの bioinformatics workflows。 | SKILLS.md files, domain workflows | Active | Medium |
| [modelscope/Awesome-Vibe-Research](https://github.com/modelscope/Awesome-Vibe-Research) | Generic Agent | vibe research と agentic research の research resources。 | Awesome list, research workflows | Active | Low |
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | ChatGPT, OpenAI API, Generic Agent | agent workflows に適用できる examples と guides。 | Examples, notebooks, API workflows | Active | Low |
| [simonw/llm](https://github.com/simonw/llm) | Generic Agent, CLI | command-line LLM workflows と plugin-backed research tasks。 | CLI, plugins, templates | Active | Medium |

## MCP and Tool Integration

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) | MCP | tool-backed agent capabilities のための reference MCP servers。 | MCP servers, examples | Active | Medium |
| [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | MCP | MCP servers の大規模な厳選コレクション。 | Awesome list, categories | Active | Medium |
| [appcypher/awesome-mcp-servers](https://github.com/appcypher/awesome-mcp-servers) | MCP | MCP servers と tool-use capabilities の厳選リスト。 | Awesome list, server links | Active | Medium |
| [jaw9c/awesome-remote-mcp-servers](https://github.com/jaw9c/awesome-remote-mcp-servers) | MCP | remote MCP server discovery。 | Awesome list, remote services | Active | Medium |
| [ai-boost/awesome-a2a](https://github.com/ai-boost/awesome-a2a) | A2A, MCP, Generic Agent | Agent2Agent tools、servers、clients、integrations。 | Awesome list, protocols, tooling | Active | Medium |
| [Francis-Zxp/AI-SkillHub](https://github.com/Francis-Zxp/AI-SkillHub) | Codex, Claude Code, Antigravity | skills の import と deployment のための desktop skill manager。 | Desktop app, skill import/sync | Active | Medium |
| [sametcelikbicak/rolecraft](https://github.com/sametcelikbicak/rolecraft) | Claude Code, Cursor, OpenCode | 任意の source から agent skills をインストールする zero-dependency CLI。 | CLI, installer workflow | Active | Medium |

## Business Workflows

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [enescingoz/awesome-n8n-templates](https://github.com/enescingoz/awesome-n8n-templates) | n8n, Generic Agent | AI agents と business automation 向けの大規模 workflow template collection。 | Workflow templates, integrations | Active | Medium |
| [lucaswalter/n8n-ai-automations](https://github.com/lucaswalter/n8n-ai-automations) | n8n | business tools 向けの AI automations と agent workflows。 | n8n workflows, examples | Active | Medium |
| [carta/plugins](https://github.com/carta/plugins) | Claude, Codex, Copilot, MCP | equity/startup workflows 向けの public plugins と skills。 | Plugins, MCP, skills | Active | High |
| [tale-project/tale](https://github.com/tale-project/tale) | OpenClaw, Claude Code, Codex, Cursor | 複数 AI agents 間で作業を orchestrate し delegate する。 | Orchestrator, workflows, MCP | Active | Medium |

## Personal Productivity

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Benkapner/claude-code-basecamp](https://github.com/Benkapner/claude-code-basecamp) | Claude Code | skills、commands、hooks を含む workspace setup。 | Skills, commands, hooks | Active | Medium |
| [Daaaaave/agentic-workspace-core](https://github.com/Daaaaave/agentic-workspace-core) | Claude Code, Codex | repository-native memory、skills、knowledge workflows。 | Memory, AGENTS.md, skills, llms.txt | Active | Medium |
| [WoJiSama/skill-based-architecture](https://github.com/WoJiSama/skill-based-architecture) | Cursor, Claude Code, Codex, Gemini | repo knowledge を reusable skills に蒸留する meta-skill。 | Meta-skill, project skill generation | Active | Medium |
| [JularDepick/user-thoughts.SKILL](https://github.com/JularDepick/user-thoughts.SKILL) | Codex, Claude Code, OpenCode | user input を永続的な project-bound idea repositories に整理。 | Agent skill, memory workflow | Active | Medium |
| [shiquda/skills-sync](https://github.com/shiquda/skills-sync) | Codex, Claude Code, Cursor | ローカル AI Agent Skills を sync、version、publish。 | CLI, GitHub publishing workflow | Active | Medium |
| [bardaxx/skillbook](https://github.com/bardaxx/skillbook) | Codex, Claude, Cursor | coding agents 向けの portable playbooks。 | Markdown workflows, sharing model | Active | Low |

## Use With Care

These projects can be valuable, but they involve sensitive domains such as security, trading, OSINT, privileged accounts, or agent-to-agent orchestration. Review permissions, confirmation steps, logs, and safety boundaries before using them.

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [gadievron/raptor](https://github.com/gadievron/raptor) | Claude Code | offensive/defensive security agent workflows。 | Rules, sub-agents, skills, security tools | Use with care | High |
| [matank001/cursor-security-rules](https://github.com/matank001/cursor-security-rules) | Cursor | AI-assisted development workflows のための security rules。 | Cursor rules, guardrails | Use with care | High |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | trading agents、市場調査、execution resources。 | Awesome list, MCP servers, agent skills | Use with care | High |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | OSINT MCP servers と investigative tooling。 | Awesome list, MCP resources | Use with care | High |

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
