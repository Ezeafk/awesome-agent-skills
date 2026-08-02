# Awesome Agent Skills

> 面向 AI Agent 的可复用技能、工作流和工具能力包精选导航。

语言：[English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

本列表聚焦能帮助 AI Agent 完成真实任务的可复用能力包。它不是 prompt dump。被收录项目应有明确场景、可复用结构、安装或使用说明，并能解释输入、输出和安全边界。

最后审核：2026-07-18

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
- [Security Skills](#security-skills)
- [DevOps and Cloud](#devops-and-cloud)
- [Research](#research)
- [MCP and Tool Integration](#mcp-and-tool-integration)
- [Finance Skills](#finance-skills)
- [Business Workflows](#business-workflows)
- [Personal Productivity](#personal-productivity)
- [Use With Care](#use-with-care)
- [评估方法](#评估方法)
- [Selection Criteria](#selection-criteria)

## Core Skill Registries

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [anthropics/skills](https://github.com/anthropics/skills) | Claude, Generic Agent | Agent Skills 的公开仓库。 | Skills, examples, references | Active | Low |
| [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Claude Code, MCP, Generic Agent | Anthropic 官方维护的 Claude Code plugin 目录。 | Plugins, skills, commands, agents, MCP configs | Active | Medium |
| [github/awesome-copilot](https://github.com/github/awesome-copilot) | Copilot, Generic Agent | 社区贡献的指令、Agent、Skill 和配置。 | Instructions, agents, skills, configs | Active | Low |
| [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) | Claude Code, Cursor, Copilot, Codex | 面向专业编码 Agent 的安全验证 Skill 注册表。 | Skill registry, validation, metadata | Active | Medium |
| [taishi-i/awesome-ChatGPT-repositories](https://github.com/taishi-i/awesome-ChatGPT-repositories) | ChatGPT, Codex, Claude | 通过 Claude Code skills 暴露的可搜索 AI 仓库精选列表。 | Awesome list, search workflow, skills | Active | Low |
| [JSONbored/awesome-claude](https://github.com/JSONbored/awesome-claude) | Claude, MCP, Generic Agent | Claude 工作流资产、Agent、MCP server、Skill、命令和 hook 的注册表。 | Registry, agents, skills, MCP, commands | Active | Medium |
| [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 可安装的多角色 AI agency 专家库，覆盖编码、安全、内容、产品和业务工作流。 | Agent library, install scripts, converters, examples | Active | Medium |
| [sickn33/agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) | Claude Code, Cursor, Codex, Gemini CLI | 面向多种编码 Agent 的大型可安装 agentic skills 库。 | Skill library, installer CLI, bundles, workflows | Active | Medium |
| [wshobson/agents](https://github.com/wshobson/agents) | Claude Code, Codex, Cursor, Copilot, Gemini CLI | 面向编码助手的多 harness agentic plugin marketplace。 | Agents, workflows, plugins, MCP configs | Active | Medium |
| [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) | Generic Agent, Claude, Codex | Vercel 官方 agent skills 集合。 | Skills, examples, workflows | Active | Medium |
| [farion1231/cc-switch](https://github.com/farion1231/cc-switch) | Claude Code, Codex, OpenCode, Gemini CLI | 面向多种编码 Agent 的桌面端 skills 与 provider 管理器。 | Desktop app, skills management, provider switching | Active | Medium |
| [microsoft/SkillOpt](https://github.com/microsoft/SkillOpt) | Codex, Claude Code, Copilot, Cursor, Devin | 通过基于轨迹的编辑和留出验证门，持续训练、评估并改进可复用的 Agent skills。 | Skill optimizer, evals, benchmarks, plugins, WebUI | Active | High |

## Coding

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [openai/codex](https://github.com/openai/codex) | Codex | 用于仓库任务的终端编码 Agent。 | CLI, sandboxed workflows, code automation | Active | Medium |
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | Claude Code | 在终端中结合仓库上下文和 git 工作流进行 Agentic coding。 | CLI, tool workflows, coding automation | Active | Medium |
| [xai-org/grok-build](https://github.com/xai-org/grok-build) | Grok Build, Claude Code, Codex, MCP | 带 TUI、headless mode、skills、plugins、hooks、MCP 和 sandboxing 的终端编码 Agent。 | CLI, TUI, skills, plugins, MCP, hooks, sandbox | Active | Medium |
| [anthropics/claude-code-action](https://github.com/anthropics/claude-code-action) | Claude Code, GitHub | 从 GitHub Actions 运行 Claude Code 工作流。 | GitHub Action, automation workflow | Active | Medium |
| [jabrena/cursor-rules-java](https://github.com/jabrena/cursor-rules-java) | Cursor, Claude, Codex, Copilot | AI 原生的 Java 企业开发工作流。 | Rules, agents, commands, MCP servers | Active | Medium |
| [DollarDill/beads-superpowers](https://github.com/DollarDill/beads-superpowers) | Claude Code, Codex, OpenCode | 面向编码 Agent 的流程纪律 Skill 和持久任务记忆。 | Skills, task memory, TDD workflows | Active | Medium |
| [vosslab/vosslab-skills](https://github.com/vosslab/vosslab-skills) | Claude, Codex | 重构、代码审查、仓库维护和教育内容工作流。 | Reusable skills, workflows | Active | Medium |
| [avalonreset/legends-github](https://github.com/avalonreset/legends-github) | Claude Code, Codex, Gemini CLI | GitHub 仓库优化和社区健康工作流。 | Skills, audit workflow, metadata checks | Active | Medium |
| [Jakevin/fastcontext-agent-tools](https://github.com/Jakevin/fastcontext-agent-tools) | Codex, MCP | 使用 FastContext 进行仓库探索。 | MCP server, Codex skill | Active | Medium |
| [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Claude Code, Codex, Cursor, Copilot | 面向 AI 编码 Agent 的生产级工程 Skill 和生命周期命令。 | Skills, commands, hooks, evals, references | Active | Medium |
| [alibaba/open-code-review](https://github.com/alibaba/open-code-review) | Claude Code, Codex, Cursor, OpenCode, MCP | 通过确定性文件选择、Agent 上下文检索、规则匹配和行级结果，对 diff 或整个代码库执行精准审查。 | CLI, skills, plugins, MCP, CI, rules, benchmarks | Active | High |
| [obra/superpowers](https://github.com/obra/superpowers) | Claude Code, Codex, Cursor, Copilot | 将 Agentic 软件开发方法论封装为可组合 Skill。 | Skills framework, plugins, hooks, tests | Active | Medium |
| [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | Claude Code, Codex, Cursor, Gemini CLI | 将代码库、schema、文档和媒体转换为可查询知识图谱，供编码 Agent 使用。 | Knowledge graph, CLI, skills, tests | Active | Medium |
| [affaan-m/ECC](https://github.com/affaan-m/ECC) | Claude Code, Codex, Cursor, OpenCode | 包含 skills、记忆、安全与研究纪律的 harness 优化系统。 | Skills, memory, security workflows, MCP | Active | Medium |

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
| [chuspeeism/dashi-ppt-skill](https://github.com/chuspeeism/dashi-ppt-skill) | Claude Code, Codex, Cursor, Generic Agent | 使用多种主题生成可在浏览器中编辑的演示文稿，并导出为 HTML、PDF 和 PPTX。 | Skill, themes, templates, render scripts, exporters | Active | Medium |

## Design and Frontend

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [LingyiChen-AI/comfyui-workflow-skill](https://github.com/LingyiChen-AI/comfyui-workflow-skill) | Claude Code, Cursor, Generic Agent | 根据自然语言生成 ComfyUI workflow JSON。 | Templates, node definitions, model workflows | Active | Medium |
| [SlavaSexton/ComfyUI-Agent-Kit](https://github.com/SlavaSexton/ComfyUI-Agent-Kit) | Claude Code, Codex, Gemini CLI | 让 Agent 端到端驱动本地 ComfyUI。 | Skill, prompt recipes, templates, automation | Active | Medium |
| [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | Claude Code, Codex, Cursor, Copilot, Windsurf | 从研究与脚本创作，到素材生成、剪辑、本地化、渲染和成片质检，完成端到端 Agent 视频制作。 | 12 pipelines, 100+ tools, 700+ skills, schemas, Remotion, FFmpeg, tests | Active | High |

## Browser and Web

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | MCP | 通过 Playwright MCP 进行浏览器自动化。 | MCP server, browser tools | Active | Medium |
| [executeautomation/mcp-playwright](https://github.com/executeautomation/mcp-playwright) | MCP, Claude, Cursor | 通过 Playwright 进行浏览器和 API 自动化。 | MCP server, Playwright workflows | Active | Medium |
| [browserbase/mcp-server-browserbase](https://github.com/browserbase/mcp-server-browserbase) | MCP | 让 Agent 通过 Browserbase 和 Stagehand 控制云浏览器。 | MCP server, browser control | Active | Medium |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | 面向研究 Agent 的 OSINT 工具发现。 | Curated MCP server list | Active | High |
| [Xquik-dev/x-twitter-scraper](https://github.com/Xquik-dev/x-twitter-scraper) | Codex, Claude, MCP, Generic Agent | 执行 X 数据研究、导出、监控和需确认的操作。 Not affiliated with X Corp. | Skill, references, hosted MCP endpoint, REST API, safety gates | Active | High |

## Security Skills

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | Claude, Codex, Generic Agent | 在安装前扫描 AI Agent skills 中的恶意模式、不安全指令和安全风险。 | Security scanner, CLI, reports, examples | Active | High |
| [cisco-ai-defense/skill-scanner](https://github.com/cisco-ai-defense/skill-scanner) | Claude, Generic Agent | 在团队采用前审查 Agent Skills 的供应链和 prompt 层风险。 | Security scanner, rules, reports | Active | High |
| [snyk/agent-scan](https://github.com/snyk/agent-scan) | MCP, Generic Agent, Claude, Codex | 扫描 AI agents、MCP servers 和 agent skills 中的漏洞及高风险工具行为。 | Security scanner, CLI, rules | Active | High |
| [trailofbits/skills](https://github.com/trailofbits/skills) | Claude Code | Trail of Bits 提供的安全研究、漏洞检测和审计工作流。 | Skills, audit workflows, examples | Active | High |
| [Tencent/AI-Infra-Guard](https://github.com/Tencent/AI-Infra-Guard) | Generic Agent, MCP | 对 AI 基础设施进行红队评估，覆盖 agent、skill、MCP、jailbreak 和 LLM 安全扫描。 | Red-team platform, scanners, reports | Active | High |

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
| [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | Claude Code, Codex | 跨社交与 Web 来源生成有依据近期摘要的研究 skill。 | Skill, web research workflow, source synthesis | Active | Medium |
| [Astro-Han/karpathy-llm-wiki](https://github.com/Astro-Han/karpathy-llm-wiki) | Claude Code, Codex, Cursor, Generic Agent | 构建由 LLM 维护的持久知识库：摄取不可变来源、基于引用回答，并检查证据与链接。 | Skill, scripts, references, examples, linting | Active | Medium |
| [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | Claude Code, Codex, Cursor, Generic Agent | 面向生物、化学、医学和科研 Agent 的科学 skill 库。 | Scientific skills, databases, workflows | Active | High |

## MCP and Tool Integration

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) | MCP | 用于工具型 Agent 能力的参考 MCP server。 | MCP servers, examples | Active | Medium |
| [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | MCP | 大型 MCP server 精选集合。 | Awesome list, categories | Active | Medium |
| [appcypher/awesome-mcp-servers](https://github.com/appcypher/awesome-mcp-servers) | MCP | MCP server 和 tool-use 能力精选列表。 | Awesome list, server links | Active | Medium |
| [jaw9c/awesome-remote-mcp-servers](https://github.com/jaw9c/awesome-remote-mcp-servers) | MCP | 远程 MCP server 发现。 | Awesome list, remote services | Active | Medium |
| [ai-boost/awesome-a2a](https://github.com/ai-boost/awesome-a2a) | A2A, MCP, Generic Agent | Agent2Agent 工具、server、client 和集成。 | Awesome list, protocols, tooling | Active | Medium |

## Finance Skills

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Bookkeeper & Controller](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-bookkeeper-controller.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 日常记账、总账、月结、对账、内控、审计准备和 GAAP 合规。 | Agent skill, finance workflow, controls checklist | Active | High |
| [Financial Analyst](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-financial-analyst.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 财务建模、预测、场景分析、估值、预算 vs 实际分析和经营决策支持。 | Agent skill, modeling workflow, analysis templates | Active | High |
| [FP&A Analyst](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-fpa-analyst.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 年度预算、滚动预测、经营计划、部门预算、KPI 和月度经营复盘。 | Agent skill, planning workflow, KPI review | Active | High |
| [Investment Researcher](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-investment-researcher.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 投资研究、尽调、资产估值、组合分析、牛熊情景和投资报告。 | Agent skill, research workflow, valuation templates | Active | High |
| [Tax Strategist](https://github.com/msitarzewski/agency-agents/blob/main/finance/finance-tax-strategist.md) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | 税务筹划、多地区合规、转让定价、实体架构和税务备忘录。 | Agent skill, tax workflow, memo templates | Active | High |

## Business Workflows

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [enescingoz/awesome-n8n-templates](https://github.com/enescingoz/awesome-n8n-templates) | n8n, Generic Agent | 面向 AI Agent 和业务自动化的大型工作流模板集合。 | Workflow templates, integrations | Active | Medium |
| [lucaswalter/n8n-ai-automations](https://github.com/lucaswalter/n8n-ai-automations) | n8n | 面向业务工具的 AI 自动化和 Agent 工作流。 | n8n workflows, examples | Active | Medium |
| [googleworkspace/cli](https://github.com/googleworkspace/cli) | Claude Code, Codex, Copilot, Gemini CLI, Generic Agent | 通过 CLI 驱动的 skills、角色包和多步骤 recipes 操作 Drive、Gmail、Calendar、Sheets、Docs、Chat 等 Workspace API。 | CLI, 40+ skills, personas, recipes, structured JSON | Active | High |
| [AgriciDaniel/claude-seo](https://github.com/AgriciDaniel/claude-seo) | Claude Code, MCP, SEO, GEO | 面向技术 SEO、内容质量、schema、GEO/AEO、本地 SEO、backlinks、电商 SEO、国际 SEO 和报告生成的综合 Claude Code SEO skill suite。 | Skills, sub-agents, commands, MCP extensions, reports, tests | Active | High |
| [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | Claude Code, Codex | 面向 CRO、文案、SEO、分析和增长的营销 skills。 | Skills, marketing workflows | Active | Medium |

## Personal Productivity

| Skill | Platform | 用途 | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Benkapner/claude-code-basecamp](https://github.com/Benkapner/claude-code-basecamp) | Claude Code | 包含 Skill、命令和 hook 的工作区设置。 | Skills, commands, hooks | Active | Medium |
| [Daaaaave/agentic-workspace-core](https://github.com/Daaaaave/agentic-workspace-core) | Claude Code, Codex | 仓库原生的记忆、Skill 和知识工作流。 | Memory, AGENTS.md, skills, llms.txt | Active | Medium |
| [WoJiSama/skill-based-architecture](https://github.com/WoJiSama/skill-based-architecture) | Cursor, Claude Code, Codex, Gemini | 将仓库知识提炼为可复用 Skill 的元 Skill。 | Meta-skill, project skill generation | Active | Medium |
| [mksglu/context-mode](https://github.com/mksglu/context-mode) | Claude Code, Codex, Cursor, MCP | 通过工具输出沙箱、会话记忆、MCP 和 hooks 优化 Agent 上下文窗口。 | MCP server, hooks, skills, memory, plugins | Active | Medium |

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
