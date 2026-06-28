# Awesome Agent Skills

> Lista curada de skills, workflows e capacidades com ferramentas para AI agents.

Idiomas: [English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

Esta lista foca em capacidades reutilizáveis que ajudam AI agents a concluir tarefas reais. Ela não é um prompt dump. Um projeto listado deve ter caso de uso claro, estrutura reutilizável, instruções de instalação ou uso e contexto suficiente para explicar entradas, saídas e limites de segurança.

Última revisão: 2026-06-28

## O Que Conta Como Skill

Nesta lista, uma skill é um pacote de capacidade reutilizável para um AI agent. Ela pode incluir instruções, workflows, scripts, referências, templates, MCP servers, connectors, automação de apps locais, etapas de validação ou exemplos.

## Legenda

| Campo | Valores |
|---|---|
| Platform | Codex, Claude, ChatGPT, Cursor, Copilot, MCP, Generic Agent, n8n |
| Includes | Workflow, scripts, references, templates, MCP server, connector, app integration, examples |
| Status | Active = manutenção recente; Stable = ainda útil com atualizações mais lentas; Use with care = valioso, mas sensível |
| Risk | Low = principalmente leitura ou geração de conteúdo; Medium = arquivos, APIs, contas, automação de navegador; High = produção, segurança, exclusão, pagamentos, credenciais, ações em massa |

## Método de Avaliação

Skills são pontuadas antes da inclusão. Stars são apenas um sinal fraco; uma skill de nicho pode entrar quando resolve uma tarefa real, tem estrutura reutilizável e dá ao agent instruções ou ferramentas suficientes para executar com segurança.

| Área | Pontos | O que revisar |
|---|---:|---|
| Clareza da tarefa | 0-2 | Caso real de uso, entradas, saídas e usuário-alvo claros. |
| Estrutura reutilizável | 0-2 | Mais que um prompt: skill files, workflows, templates, scripts, examples ou references. |
| Plataforma e ferramentas | 0-2 | Suporte claro a Codex, Claude, ChatGPT, Cursor, Copilot, MCP, n8n, CLI, browser, API ou workflows de app local. |
| Validação e exemplos | 0-2 | Demo, testes, sample usage, CI checks, schema ou verificação passo a passo. |
| Manutenção e segurança | 0-2 | Atividade recente, licença clara, defaults seguros, regras de confirmação e orientação de credenciais/privacidade. |

Guia de inclusão: 8-10 = recomendado, 6-7 = aceitável com ressalvas, 4-5 = use com cuidado ou revise novamente, abaixo de 4 = remover ou não incluir. Workflows de alto risco precisam de pontuação mais forte e notas explícitas de segurança.

## Conteúdo

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
- [Business Workflows](#business-workflows)
- [Personal Productivity](#personal-productivity)
- [Use With Care](#use-with-care)
- [Método de Avaliação](#método-de-avaliação)
- [Selection Criteria](#selection-criteria)

## Core Skill Registries

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [anthropics/skills](https://github.com/anthropics/skills) | Claude, Generic Agent | Repositório público para Agent Skills. | Skills, examples, references | Active | Low |
| [github/awesome-copilot](https://github.com/github/awesome-copilot) | Copilot, Generic Agent | Instruções, agents, skills e configurações da comunidade. | Instructions, agents, skills, configs | Active | Low |
| [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) | Claude Code, Cursor, Copilot, Codex | Registro seguro e validado de skills para agentes profissionais de programação. | Skill registry, validation, metadata | Active | Medium |
| [taishi-i/awesome-ChatGPT-repositories](https://github.com/taishi-i/awesome-ChatGPT-repositories) | ChatGPT, Codex, Claude | Lista curada e pesquisável de repositórios de IA exposta por Claude Code skills. | Awesome list, search workflow, skills | Active | Low |
| [JSONbored/awesome-claude](https://github.com/JSONbored/awesome-claude) | Claude, MCP, Generic Agent | Registro de assets de workflow do Claude, agents, MCP servers, skills, comandos e hooks. | Registry, agents, skills, MCP, commands | Active | Medium |
| [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | Claude Code, Copilot, Cursor, Codex, Gemini CLI, OpenCode, Aider, Windsurf | Biblioteca instalável de agência de IA com especialistas para codificação, segurança, conteúdo, produto e fluxos de trabalho de negócios. | Agent library, install scripts, converters, examples | Active | Medium |

## Coding

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [openai/codex](https://github.com/openai/codex) | Codex | Agente de programação no terminal para tarefas de repositório. | CLI, sandboxed workflows, code automation | Active | Medium |
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | Claude Code | Programação agentic no terminal com contexto do repositório e workflows git. | CLI, tool workflows, coding automation | Active | Medium |
| [anthropics/claude-code-action](https://github.com/anthropics/claude-code-action) | Claude Code, GitHub | Executar workflows do Claude Code a partir do GitHub Actions. | GitHub Action, automation workflow | Active | Medium |
| [jabrena/cursor-rules-java](https://github.com/jabrena/cursor-rules-java) | Cursor, Claude, Codex, Copilot | Workflow de desenvolvimento Java empresarial nativo para IA. | Rules, agents, commands, MCP servers | Active | Medium |
| [DollarDill/beads-superpowers](https://github.com/DollarDill/beads-superpowers) | Claude Code, Codex, OpenCode | Skills de disciplina de processo e memória persistente de tarefas para agentes de programação. | Skills, task memory, TDD workflows | Active | Medium |
| [vosslab/vosslab-skills](https://github.com/vosslab/vosslab-skills) | Claude, Codex | Workflows de refatoração, revisão de código, manutenção de repositório e conteúdo educacional. | Reusable skills, workflows | Active | Medium |
| [avalonreset/legends-github](https://github.com/avalonreset/legends-github) | Claude Code, Codex, Gemini CLI | Workflows de otimização de repositórios GitHub e saúde da comunidade. | Skills, audit workflow, metadata checks | Active | Medium |
| [Jakevin/fastcontext-agent-tools](https://github.com/Jakevin/fastcontext-agent-tools) | Codex, MCP | Exploração de repositórios com FastContext. | MCP server, Codex skill | Active | Medium |

## Data Analysis

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Kaelio/ktx](https://github.com/Kaelio/ktx) | Claude, Codex, MCP | Camada de contexto executável para agentes de analytics. | Semantic context, database querying, MCP | Active | Medium |
| [dagster-io/dagster](https://github.com/dagster-io/dagster) | Generic Agent | Orquestração de data assets para workflows analíticos guiados por agentes. | Pipelines, schedules, observability | Active | Medium |
| [EtienneLescot/n8n-as-code](https://github.com/EtienneLescot/n8n-as-code) | n8n, Claude, Cursor, Copilot | Dar aos agentes capacidades de criação e sincronização de workflows n8n. | TypeScript workflows, schemas, templates | Active | Medium |
| [product-on-purpose/pm-skills](https://github.com/product-on-purpose/pm-skills) | Claude, Codex | Famílias de skills de product management e workflows estruturados de produto. | Skills, templates, examples, CI contracts | Active | Medium |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | Skills de pesquisa de mercado, estratégia e agentes de trading. | Awesome list, MCP servers, workflows | Active | High |

## Documents

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [yusufkaraaslan/Skill_Seekers](https://github.com/yusufkaraaslan/Skill_Seekers) | Claude | Converter docs, repositórios GitHub e PDFs em Claude skills. | Parser, OCR, conflict detection, MCP | Active | Medium |
| [teng-lin/notebooklm-py](https://github.com/teng-lin/notebooklm-py) | Claude, Codex, Python | Workflows programáticos do NotebookLM para agentes. | Python API, CLI, agentic skill | Active | Medium |

## Design and Frontend

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [LingyiChen-AI/comfyui-workflow-skill](https://github.com/LingyiChen-AI/comfyui-workflow-skill) | Claude Code, Cursor, Generic Agent | Gerar JSON de workflow ComfyUI a partir de linguagem natural. | Templates, node definitions, model workflows | Active | Medium |
| [SlavaSexton/ComfyUI-Agent-Kit](https://github.com/SlavaSexton/ComfyUI-Agent-Kit) | Claude Code, Codex, Gemini CLI | Controlar o ComfyUI local de ponta a ponta a partir de um agente. | Skill, prompt recipes, templates, automation | Active | Medium |

## Browser and Web

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [microsoft/playwright-mcp](https://github.com/microsoft/playwright-mcp) | MCP | Automação de navegador através do Playwright MCP. | MCP server, browser tools | Active | Medium |
| [executeautomation/mcp-playwright](https://github.com/executeautomation/mcp-playwright) | MCP, Claude, Cursor | Automação de navegador e API através do Playwright. | MCP server, Playwright workflows | Active | Medium |
| [browserbase/mcp-server-browserbase](https://github.com/browserbase/mcp-server-browserbase) | MCP | Permitir que agentes controlem navegadores em nuvem com Browserbase e Stagehand. | MCP server, browser control | Active | Medium |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | Descoberta de ferramentas OSINT para agentes de pesquisa. | Curated MCP server list | Active | High |

## Security Skills

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | Claude, Codex, Generic Agent | Escanear AI agent skills antes da instalação para detectar padrões maliciosos, instruções inseguras e riscos de segurança. | Security scanner, CLI, reports, examples | Active | High |
| [cisco-ai-defense/skill-scanner](https://github.com/cisco-ai-defense/skill-scanner) | Claude, Generic Agent | Avaliar Agent Skills quanto a riscos de cadeia de suprimentos e de prompt antes da adoção por equipes. | Security scanner, rules, reports | Active | High |
| [snyk/agent-scan](https://github.com/snyk/agent-scan) | MCP, Generic Agent, Claude, Codex | Escanear AI agents, MCP servers e agent skills em busca de vulnerabilidades e comportamentos arriscados de ferramentas. | Security scanner, CLI, rules | Active | High |
| [trailofbits/skills](https://github.com/trailofbits/skills) | Claude Code | Workflows da Trail of Bits para pesquisa de segurança, detecção de vulnerabilidades e auditoria. | Skills, audit workflows, examples | Active | High |
| [Tencent/AI-Infra-Guard](https://github.com/Tencent/AI-Infra-Guard) | Generic Agent, MCP | Fazer red team de infraestrutura de IA com varreduras de agent, skill, MCP, jailbreak e segurança de LLM. | Red-team platform, scanners, reports | Active | High |

## DevOps and Cloud

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [rohitg00/awesome-devops-mcp-servers](https://github.com/rohitg00/awesome-devops-mcp-servers) | MCP, DevOps | MCP servers e capacidades focadas em DevOps. | Curated MCP list, ops tools | Active | High |
| [Azure/awesome-azd](https://github.com/Azure/awesome-azd) | Azure, Generic Agent | Templates e workflows do Azure Developer CLI. | Templates, docs, deployment examples | Active | Medium |
| [AmoyLab/Unla](https://github.com/AmoyLab/Unla) | MCP | Transformar APIs e MCP servers em capacidades MCP gerenciadas. | Gateway, UI, Docker deployment | Active | Medium |
| [milisp/mcp-linker](https://github.com/milisp/mcp-linker) | MCP, Claude, Cursor | Sincronizar configurações de MCP server entre clientes. | MCP manager, config sync | Active | Medium |
| [hashgraph-online/hol-guard](https://github.com/hashgraph-online/hol-guard) | Codex, Claude Code, Cursor, MCP | Escanear plugins, skills e MCP servers antes da execução de ferramentas. | Security scanner, CLI, policy checks | Active | High |

## Research

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [GPTomics/bioSkills](https://github.com/GPTomics/bioSkills) | Claude Code, Generic Agent | Workflows de bioinformática para agentes de programação. | SKILLS.md files, domain workflows | Active | Medium |
| [modelscope/Awesome-Vibe-Research](https://github.com/modelscope/Awesome-Vibe-Research) | Generic Agent | Recursos de pesquisa para vibe research e agentic research. | Awesome list, research workflows | Active | Low |
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | ChatGPT, OpenAI API, Generic Agent | Exemplos e guias que podem ser adaptados para workflows de agentes. | Examples, notebooks, API workflows | Active | Low |
| [simonw/llm](https://github.com/simonw/llm) | Generic Agent, CLI | Workflows LLM de linha de comando e tarefas de pesquisa apoiadas por plugins. | CLI, plugins, templates | Active | Medium |

## MCP and Tool Integration

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) | MCP | MCP servers de referência para capacidades de agentes com ferramentas. | MCP servers, examples | Active | Medium |
| [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | MCP | Grande coleção curada de MCP servers. | Awesome list, categories | Active | Medium |
| [appcypher/awesome-mcp-servers](https://github.com/appcypher/awesome-mcp-servers) | MCP | Lista curada de MCP servers e capacidades de tool-use. | Awesome list, server links | Active | Medium |
| [jaw9c/awesome-remote-mcp-servers](https://github.com/jaw9c/awesome-remote-mcp-servers) | MCP | Descoberta de MCP servers remotos. | Awesome list, remote services | Active | Medium |
| [ai-boost/awesome-a2a](https://github.com/ai-boost/awesome-a2a) | A2A, MCP, Generic Agent | Ferramentas, servers, clients e integrações Agent2Agent. | Awesome list, protocols, tooling | Active | Medium |

## Business Workflows

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [enescingoz/awesome-n8n-templates](https://github.com/enescingoz/awesome-n8n-templates) | n8n, Generic Agent | Grande coleção de templates de workflow para AI agents e automação de negócios. | Workflow templates, integrations | Active | Medium |
| [lucaswalter/n8n-ai-automations](https://github.com/lucaswalter/n8n-ai-automations) | n8n | Automações de IA e workflows de agentes para ferramentas de negócios. | n8n workflows, examples | Active | Medium |

## Personal Productivity

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [Benkapner/claude-code-basecamp](https://github.com/Benkapner/claude-code-basecamp) | Claude Code | Configuração de workspace com skills, comandos e hooks. | Skills, commands, hooks | Active | Medium |
| [Daaaaave/agentic-workspace-core](https://github.com/Daaaaave/agentic-workspace-core) | Claude Code, Codex | Memória, skills e workflows de conhecimento nativos do repositório. | Memory, AGENTS.md, skills, llms.txt | Active | Medium |
| [WoJiSama/skill-based-architecture](https://github.com/WoJiSama/skill-based-architecture) | Cursor, Claude Code, Codex, Gemini | Meta-skill que destila conhecimento do repositório em skills reutilizáveis. | Meta-skill, project skill generation | Active | Medium |

## Use With Care

These projects can be valuable, but they involve sensitive domains such as security, trading, OSINT, privileged accounts, or agent-to-agent orchestration. Review permissions, confirmation steps, logs, and safety boundaries before using them.

| Skill | Platform | Caso de uso | Includes | Status | Risk |
|---|---|---|---|---|---|
| [gadievron/raptor](https://github.com/gadievron/raptor) | Claude Code | Workflows de agentes de segurança ofensiva e defensiva. | Rules, sub-agents, skills, security tools | Use with care | High |
| [matank001/cursor-security-rules](https://github.com/matank001/cursor-security-rules) | Cursor | Regras de segurança para workflows de desenvolvimento assistido por IA. | Cursor rules, guardrails | Use with care | High |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Generic Agent, MCP | Agentes de trading, pesquisa de mercado e recursos de execução. | Awesome list, MCP servers, agent skills | Use with care | High |
| [soxoj/awesome-osint-mcp-servers](https://github.com/soxoj/awesome-osint-mcp-servers) | MCP | MCP servers OSINT e ferramentas investigativas. | Awesome list, MCP resources | Use with care | High |

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
