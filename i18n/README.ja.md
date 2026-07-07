# Awesome Agent Skills

> AI agents 向けの再利用可能な skills、workflows、tool-backed capabilities の厳選リスト。

言語: [English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

このリストは、AI agents が実際のタスクを完了するための再利用可能な能力に焦点を当てています。prompt dump ではありません。掲載プロジェクトには明確なユースケース、再利用可能な構造、インストールまたは利用手順、入力・出力・安全境界を説明できる情報が必要です。

最終確認日: 2026-07-07

## Skill の定義

このリストでは、skill は AI agent のための再利用可能な能力パッケージです。instructions、workflows、scripts、references、templates、MCP servers、connectors、local app automation、validation steps、examples などを含みます。

## 凡例

| 項目 | 値 |
|---|---|
| Platform | Codex, Claude, ChatGPT, Cursor, Copilot, MCP, Generic Agent, n8n |
| Includes | Workflow, scripts, references, templates, MCP server, connector, app integration, examples |
| Status | Active = 最近メンテナンスあり；Stable = 更新は遅いが有用；Use with care = 有用だが慎重な扱いが必要 |
| Risk | Low = 主に読み取りまたはコンテンツ生成；Medium = files、APIs、accounts、browser automation；High = production、security、deletion、payments、credentials、bulk actions |

## 評価方法

Skills は掲載前にスコアリングします。Stars は弱いシグナルにすぎません。ニッチな skill でも、実タスクを解決し、再利用可能な構造があり、agents が安全に実行できる十分な instructions や tools があれば掲載できます。

| 領域 | 点数 | 確認内容 |
|---|---:|---|
| タスク明確性 | 0-2 | 明確な実ユースケース、inputs、outputs、対象ユーザー。 |
| 再利用可能な構造 | 0-2 | prompt 以上のもの: skill files、workflows、templates、scripts、examples、references。 |
| Platform と tool の適合 | 0-2 | Codex、Claude、ChatGPT、Cursor、Copilot、MCP、n8n、CLI、browser、API、local app workflows の明確な対応。 |
| 検証と例 | 0-2 | Demo、tests、sample usage、CI checks、schema、または step-by-step verification。 |
| メンテナンスと安全性 | 0-2 | 最近の activity、明確な license、安全な defaults、confirmation rules、credential/privacy guidance。 |

掲載目安: 8-10 = 推奨、6-7 = 注意付きで可、4-5 = Use with care または再審査、4 未満 = 削除または掲載しない。高リスク workflows にはより高いスコアと明確な安全メモが必要です。

## 目次

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
- [評価方法](#評価方法)
- [Selection Criteria](#selection-criteria)

## Core Skill Registries

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [anthropics/skills](https://github.com/anthropics/skills) | Claude, Generic Agent | Agent Skills の公開リポジトリ。 | Skills, examples, references | Active | Low |
| [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Claude Code, MCP, Generic Agent | Anthropic が公式に管理する Claude Code plugin ディレクトリ。 | Plugins, skills, commands, agents, MCP configs | Active | Medium |
| [github/awesome-copilot](https://github.com/github/awesome-copilot) | Copilot, Generic Agent | コミュニティによる instructions、agents、skills、configurations。 | Instructions, agents, skills, configs | Active | Low |
| [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) | Claude Code, Cursor, Copilot, Codex | プロ向け coding agents のための安全に検証された skill registry。 | Skill registry, validation, metadata | Active | Medium |
| [taishi-i/awesome-ChatGPT-repositories](https://github.com/taishi-i/awesome-ChatGPT-repositories) | ChatGPT, Codex, Claude | Claude Code skills から利用できる検索可能な AI リポジトリ厳選リスト。 | Awesome list, search workflow, skills | Active | Low |
| [JSONbored/awesome-claude](https://github.com/JSONbored/awesome-claude) | Claude, MCP, Generic Agent | Claude workflow assets、agents、MCP servers、skills、commands、hooks の registry。 | Registry, agents, skills, MCP, commands | Active | Medium |
| [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | コーディング、セキュリティ、コンテンツ、プロダクト、業務ワークフロー向けのインストール可能な多役割 AI エージェンシーライブラリ。 | Agent library, install scripts, converters, examples | Active | Medium |

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
| [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Claude Code, Codex, Cursor, Copilot | AI coding agent 向けの本番品質エンジニアリング Skill とライフサイクルコマンド。 | Skills, commands, hooks, evals, references | Active | Medium |
| [obra/superpowers](https://github.com/obra/superpowers) | Claude Code, Codex, Cursor, Copilot | Agentic software development 方法論を組み合わせ可能な Skill として提供。 | Skills framework, plugins, hooks, tests | Active | Medium |
| [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | Claude Code, Codex, Cursor, Gemini CLI | codebase、schema、docs、media を coding agent 用の検索可能な knowledge graph に変換。 | Knowledge graph, CLI, skills, tests | Active | Medium |

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

## Design and Frontend

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [LingyiChen-AI/comfyui-workflow-skill](https://github.com/LingyiChen-AI/comfyui-workflow-skill) | Claude Code, Cursor, Generic Agent | 自然言語から ComfyUI workflow JSON を生成。 | Templates, node definitions, model workflows | Active | Medium |
| [SlavaSexton/ComfyUI-Agent-Kit](https://github.com/SlavaSexton/ComfyUI-Agent-Kit) | Claude Code, Codex, Gemini CLI | agent からローカル ComfyUI をエンドツーエンドで操作。 | Skill, prompt recipes, templates, automation | Active | Medium |

## Browser and Web

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | MCP | Playwright MCP による browser automation。 | MCP server, browser tools | Active | Medium |
| [executeautomation/mcp-playwright](https://github.com/executeautomation/mcp-playwright) | MCP, Claude, Cursor | Playwright による browser と API automation。 | MCP server, Playwright workflows | Active | Medium |
| [browserbase/mcp-server-browserbase](https://github.com/browserbase/mcp-server-browserbase) | MCP | Browserbase と Stagehand で agents が cloud browsers を制御できるようにする。 | MCP server, browser control | Active | Medium |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | research agents 向けの OSINT tool discovery。 | Curated MCP server list | Active | High |

## Security Skills

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | Claude, Codex, Generic Agent | インストール前に AI agent skills の悪意あるパターン、不安全な指示、セキュリティリスクをスキャン。 | Security scanner, CLI, reports, examples | Active | High |
| [cisco-ai-defense/skill-scanner](https://github.com/cisco-ai-defense/skill-scanner) | Claude, Generic Agent | チーム導入前に Agent Skills のサプライチェーンリスクと prompt レベルのリスクを評価。 | Security scanner, rules, reports | Active | High |
| [snyk/agent-scan](https://github.com/snyk/agent-scan) | MCP, Generic Agent, Claude, Codex | AI agents、MCP servers、agent skills の脆弱性や危険な tool 挙動をスキャン。 | Security scanner, CLI, rules | Active | High |
| [trailofbits/skills](https://github.com/trailofbits/skills) | Claude Code | Trail of Bits によるセキュリティ調査、脆弱性検出、監査ワークフロー。 | Skills, audit workflows, examples | Active | High |
| [Tencent/AI-Infra-Guard](https://github.com/Tencent/AI-Infra-Guard) | Generic Agent, MCP | agent、skill、MCP、jailbreak、LLM セキュリティスキャンで AI インフラを red-team 評価。 | Red-team platform, scanners, reports | Active | High |

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

## Finance Skills

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Bookkeeper & Controller](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-bookkeeper-controller.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 日次記帳、総勘定元帳、月次決算、照合、内部統制、監査準備、GAAP 準拠。 | Agent skill, finance workflow, controls checklist | Active | High |
| [Financial Analyst](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-financial-analyst.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 財務モデリング、予測、シナリオ分析、バリュエーション、予実分析、経営判断支援。 | Agent skill, modeling workflow, analysis templates | Active | High |
| [FP&A Analyst](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-fpa-analyst.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 年次予算、ローリングフォーキャスト、事業計画、部門予算、KPI、月次事業レビュー。 | Agent skill, planning workflow, KPI review | Active | High |
| [Investment Researcher](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-investment-researcher.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 投資リサーチ、デューデリジェンス、資産評価、ポートフォリオ分析、強気/弱気シナリオ、投資メモ。 | Agent skill, research workflow, valuation templates | Active | High |
| [Tax Strategist](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-tax-strategist.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 税務プランニング、複数地域のコンプライアンス、移転価格、法人構造設計、税務メモ。 | Agent skill, tax workflow, memo templates | Active | High |

## Business Workflows

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [enescingoz/awesome-n8n-templates](https://github.com/enescingoz/awesome-n8n-templates) | n8n, Generic Agent | AI agents と business automation 向けの大規模 workflow template collection。 | Workflow templates, integrations | Active | Medium |
| [lucaswalter/n8n-ai-automations](https://github.com/lucaswalter/n8n-ai-automations) | n8n | business tools 向けの AI automations と agent workflows。 | n8n workflows, examples | Active | Medium |

## Personal Productivity

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Benkapner/claude-code-basecamp](https://github.com/Benkapner/claude-code-basecamp) | Claude Code | skills、commands、hooks を含む workspace setup。 | Skills, commands, hooks | Active | Medium |
| [Daaaaave/agentic-workspace-core](https://github.com/Daaaaave/agentic-workspace-core) | Claude Code, Codex | repository-native memory、skills、knowledge workflows。 | Memory, AGENTS.md, skills, llms.txt | Active | Medium |
| [WoJiSama/skill-based-architecture](https://github.com/WoJiSama/skill-based-architecture) | Cursor, Claude Code, Codex, Gemini | repo knowledge を reusable skills に蒸留する meta-skill。 | Meta-skill, project skill generation | Active | Medium |
| [mksglu/context-mode](https://github.com/mksglu/context-mode) | Claude Code, Codex, Cursor, MCP | tool 出力 sandbox、session memory、MCP、hooks で agent の context window を最適化。 | MCP server, hooks, skills, memory, plugins | Active | Medium |

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
