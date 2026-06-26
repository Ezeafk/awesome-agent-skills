# Awesome Agent Skills

> 面向 AI Agent 的可复用技能、工作流和工具能力包精选导航。

语言：[English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

本列表聚焦能帮助 AI Agent 完成真实任务的可复用能力包。它不是 prompt dump。被收录项目应有明确场景、可复用结构、安装或使用说明，并能解释输入、输出和安全边界。

最后审核：2026-06-26

## 什么算 Skill

在本列表中，skill 指 AI Agent 可复用的能力包。它可以包含指令、工作流、脚本、参考资料、模板、MCP server、connector、本地应用自动化、验证步骤或示例。

## 标记说明

| 字段 | 含义 |
|---|---|
| Platform | Codex, Claude, ChatGPT, Cursor, Copilot, MCP, Generic Agent, n8n |
| Includes | Workflow、scripts、references、templates、MCP server、connector、app integration、examples |
| Status | Active = 近期有维护；Stable = 更新较慢但仍可用；Use with care = 有价值但较敏感 |
| Risk | Low = 多为只读或内容生成；Medium = 文件、API、账号、浏览器自动化；High = 生产环境、安全、删除、支付、凭证、批量操作 |

## 评估方法

Skill 收录前需要评分。Star 只是弱信号；小众 skill 如果能解决真实任务、有可复用结构，并给 Agent 足够的执行说明或工具，也可以收录。

| 维度 | 分值 | 审核重点 |
|---|---:|---|
| 任务清晰度 | 0-2 | 是否有明确真实场景、输入、输出和目标用户。 |
| 可复用结构 | 0-2 | 是否不只是 prompt，而是包含 skill 文件、workflow、template、script、example 或 reference。 |
| 平台与工具适配 | 0-2 | 是否明确支持 Codex、Claude、ChatGPT、Cursor、Copilot、MCP、n8n、CLI、浏览器、API 或本地应用工作流。 |
| 验证与示例 | 0-2 | 是否有 demo、test、sample usage、CI check、schema 或逐步验证流程。 |
| 维护与安全 | 0-2 | 是否有近期维护、清晰 license、安全默认值、确认机制和凭证/隐私说明。 |

收录参考：8-10 分推荐收录，6-7 分可带说明收录，4-5 分放入谨慎使用或复审，低于 4 分移除或暂不收录。高风险工作流必须有更高分和明确安全说明。

## 目录

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
- [评估方法](#评估方法)
- [Selection Criteria](#selection-criteria)

## Core Skill Registries

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [anthropics/skills](https://github.com/anthropics/skills) | Claude, Generic Agent | Agent Skills 的公开仓库。 | Skills, examples, references | Active | Low |
| [github/awesome-copilot](https://github.com/github/awesome-copilot) | Copilot, Generic Agent | 社区贡献的指令、Agent、Skill 和配置。 | Instructions, agents, skills, configs | Active | Low |
| [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) | Claude Code, Cursor, Copilot, Codex | 面向专业编码 Agent 的安全验证 Skill 注册表。 | Skill registry, validation, metadata | Active | Medium |
| [taishi-i/awesome-ChatGPT-repositories](https://github.com/taishi-i/awesome-ChatGPT-repositories) | ChatGPT, Codex, Claude | 通过 Claude Code skills 暴露的可搜索 AI 仓库精选列表。 | Awesome list, search workflow, skills | Active | Low |
| [JSONbored/awesome-claude](https://github.com/JSONbored/awesome-claude) | Claude, MCP, Generic Agent | Claude 工作流资产、Agent、MCP server、Skill、命令和 hook 的注册表。 | Registry, agents, skills, MCP, commands | Active | Medium |

## Coding

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [openai/codex](https://github.com/openai/codex) | Codex | 用于仓库任务的终端编码 Agent。 | CLI, sandboxed workflows, code automation | Active | Medium |
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | Claude Code | 在终端中结合仓库上下文和 git 工作流进行 Agentic coding。 | CLI, tool workflows, coding automation | Active | Medium |
| [anthropics/claude-code-action](https://github.com/anthropics/claude-code-action) | Claude Code, GitHub | 从 GitHub Actions 运行 Claude Code 工作流。 | GitHub Action, automation workflow | Active | Medium |
| [jabrena/cursor-rules-java](https://github.com/jabrena/cursor-rules-java) | Cursor, Claude, Codex, Copilot | AI 原生的 Java 企业开发工作流。 | Rules, agents, commands, MCP servers | Active | Medium |
| [DollarDill/beads-superpowers](https://github.com/DollarDill/beads-superpowers) | Claude Code, Codex, OpenCode | 面向编码 Agent 的流程纪律 Skill 和持久任务记忆。 | Skills, task memory, TDD workflows | Active | Medium |
| [vosslab/vosslab-skills](https://github.com/vosslab/vosslab-skills) | Claude, Codex | 重构、代码审查、仓库维护和教育内容工作流。 | Reusable skills, workflows | Active | Medium |
| [avalonreset/legends-github](https://github.com/avalonreset/legends-github) | Claude Code, Codex, Gemini CLI | GitHub 仓库优化和社区健康工作流。 | Skills, audit workflow, metadata checks | Active | Medium |
| [Jakevin/fastcontext-agent-tools](https://github.com/Jakevin/fastcontext-agent-tools) | Codex, MCP | 使用 FastContext 进行仓库探索。 | MCP server, Codex skill | Active | Medium |

## Data Analysis

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Kaelio/ktx](https://github.com/Kaelio/ktx) | Claude, Codex, MCP | 面向分析 Agent 的可执行上下文层。 | Semantic context, database querying, MCP | Active | Medium |
| [dagster-io/dagster](https://github.com/dagster-io/dagster) | Generic Agent | 面向 Agent 驱动分析工作流的数据资产编排。 | Pipelines, schedules, observability | Active | Medium |
| [EtienneLescot/n8n-as-code](https://github.com/EtienneLescot/n8n-as-code) | n8n, Claude, Cursor, Copilot | 为 Agent 提供 n8n 工作流创建和同步能力。 | TypeScript workflows, schemas, templates | Active | Medium |
| [product-on-purpose/pm-skills](https://github.com/product-on-purpose/pm-skills) | Claude, Codex | 产品管理 Skill 家族和结构化产品工作流。 | Skills, templates, examples, CI contracts | Active | Medium |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | 市场研究、策略和交易 Agent Skill。 | Awesome list, MCP servers, workflows | Active | High |

## Documents

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [yusufkaraaslan/Skill_Seekers](https://github.com/yusufkaraaslan/Skill_Seekers) | Claude | 将文档、GitHub 仓库和 PDF 转换为 Claude skills。 | Parser, OCR, conflict detection, MCP | Active | Medium |
| [teng-lin/notebooklm-py](https://github.com/teng-lin/notebooklm-py) | Claude, Codex, Python | 面向 Agent 的 NotebookLM 编程式工作流。 | Python API, CLI, agentic skill | Active | Medium |

## Design and Frontend

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [LingyiChen-AI/comfyui-workflow-skill](https://github.com/LingyiChen-AI/comfyui-workflow-skill) | Claude Code, Cursor, Generic Agent | 根据自然语言生成 ComfyUI workflow JSON。 | Templates, node definitions, model workflows | Active | Medium |
| [SlavaSexton/ComfyUI-Agent-Kit](https://github.com/SlavaSexton/ComfyUI-Agent-Kit) | Claude Code, Codex, Gemini CLI | 让 Agent 端到端驱动本地 ComfyUI。 | Skill, prompt recipes, templates, automation | Active | Medium |

## Browser and Web

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | MCP | 通过 Playwright MCP 进行浏览器自动化。 | MCP server, browser tools | Active | Medium |
| [executeautomation/mcp-playwright](https://github.com/executeautomation/mcp-playwright) | MCP, Claude, Cursor | 通过 Playwright 进行浏览器和 API 自动化。 | MCP server, Playwright workflows | Active | Medium |
| [browserbase/mcp-server-browserbase](https://github.com/browserbase/mcp-server-browserbase) | MCP | 让 Agent 通过 Browserbase 和 Stagehand 控制云浏览器。 | MCP server, browser control | Active | Medium |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | 面向研究 Agent 的 OSINT 工具发现。 | Curated MCP server list | Active | High |

## DevOps and Cloud

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [rohitg00/awesome-devops-mcp-servers](https://github.com/rohitg00/awesome-devops-mcp-servers) | MCP, DevOps | 聚焦 DevOps 的 MCP server 和能力。 | Curated MCP list, ops tools | Active | High |
| [Azure/awesome-azd](https://github.com/Azure/awesome-azd) | Azure, Generic Agent | Azure Developer CLI 模板和工作流。 | Templates, docs, deployment examples | Active | Medium |
| [AmoyLab/Unla](https://github.com/AmoyLab/Unla) | MCP | 将 API 和 MCP server 转换为托管 MCP 能力。 | Gateway, UI, Docker deployment | Active | Medium |
| [milisp/mcp-linker](https://github.com/milisp/mcp-linker) | MCP, Claude, Cursor | 在多个客户端之间同步 MCP server 配置。 | MCP manager, config sync | Active | Medium |
| [hashgraph-online/hol-guard](https://github.com/hashgraph-online/hol-guard) | Codex, Claude Code, Cursor, MCP | 在工具运行前扫描插件、Skill 和 MCP server。 | Security scanner, CLI, policy checks | Active | High |

## Research

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [GPTomics/bioSkills](https://github.com/GPTomics/bioSkills) | Claude Code, Generic Agent | 面向编码 Agent 的生物信息学工作流。 | SKILLS.md files, domain workflows | Active | Medium |
| [modelscope/Awesome-Vibe-Research](https://github.com/modelscope/Awesome-Vibe-Research) | Generic Agent | vibe research 和 agentic research 的研究资源。 | Awesome list, research workflows | Active | Low |
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | ChatGPT, OpenAI API, Generic Agent | 可改造为 Agent 工作流的示例和指南。 | Examples, notebooks, API workflows | Active | Low |
| [simonw/llm](https://github.com/simonw/llm) | Generic Agent, CLI | 命令行 LLM 工作流和插件支持的研究任务。 | CLI, plugins, templates | Active | Medium |

## MCP and Tool Integration

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) | MCP | 用于工具型 Agent 能力的参考 MCP server。 | MCP servers, examples | Active | Medium |
| [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | MCP | 大型 MCP server 精选集合。 | Awesome list, categories | Active | Medium |
| [appcypher/awesome-mcp-servers](https://github.com/appcypher/awesome-mcp-servers) | MCP | MCP server 和 tool-use 能力精选列表。 | Awesome list, server links | Active | Medium |
| [jaw9c/awesome-remote-mcp-servers](https://github.com/jaw9c/awesome-remote-mcp-servers) | MCP | 远程 MCP server 发现。 | Awesome list, remote services | Active | Medium |
| [ai-boost/awesome-a2a](https://github.com/ai-boost/awesome-a2a) | A2A, MCP, Generic Agent | Agent2Agent 工具、server、client 和集成。 | Awesome list, protocols, tooling | Active | Medium |

## Business Workflows

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [enescingoz/awesome-n8n-templates](https://github.com/enescingoz/awesome-n8n-templates) | n8n, Generic Agent | 面向 AI Agent 和业务自动化的大型工作流模板集合。 | Workflow templates, integrations | Active | Medium |
| [lucaswalter/n8n-ai-automations](https://github.com/lucaswalter/n8n-ai-automations) | n8n | 面向业务工具的 AI 自动化和 Agent 工作流。 | n8n workflows, examples | Active | Medium |

## Personal Productivity

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Benkapner/claude-code-basecamp](https://github.com/Benkapner/claude-code-basecamp) | Claude Code | 包含 Skill、命令和 hook 的工作区设置。 | Skills, commands, hooks | Active | Medium |
| [Daaaaave/agentic-workspace-core](https://github.com/Daaaaave/agentic-workspace-core) | Claude Code, Codex | 仓库原生的记忆、Skill 和知识工作流。 | Memory, AGENTS.md, skills, llms.txt | Active | Medium |
| [WoJiSama/skill-based-architecture](https://github.com/WoJiSama/skill-based-architecture) | Cursor, Claude Code, Codex, Gemini | 将仓库知识提炼为可复用 Skill 的元 Skill。 | Meta-skill, project skill generation | Active | Medium |

## Use With Care

These projects can be valuable, but they involve sensitive domains such as security, trading, OSINT, privileged accounts, or agent-to-agent orchestration. Review permissions, confirmation steps, logs, and safety boundaries before using them.

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [gadievron/raptor](https://github.com/gadievron/raptor) | Claude Code | 攻防安全 Agent 工作流。 | Rules, sub-agents, skills, security tools | Use with care | High |
| [matank001/cursor-security-rules](https://github.com/matank001/cursor-security-rules) | Cursor | 面向 AI 辅助开发工作流的安全规则。 | Cursor rules, guardrails | Use with care | High |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | 交易 Agent、市场研究和执行资源。 | Awesome list, MCP servers, agent skills | Use with care | High |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | OSINT MCP server 和调查工具。 | Awesome list, MCP resources | Use with care | High |

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
