# Contributing

Thanks for helping improve Awesome Agent Skills.

This list is intentionally not a prompt dump. Please submit reusable capabilities that help agents complete real tasks.

## Before Submitting

Make sure the project:

- Has a clear use case.
- Has reusable structure beyond a single prompt.
- Explains installation, copying, or usage.
- States the platform or runtime.
- Makes inputs and outputs understandable.
- Includes safety notes if it touches files, accounts, browsers, APIs, production systems, security tools, payments, or bulk messaging.

## Entry Format

Use the existing table format:

```md
| [Skill](https://github.com/owner/repo) | Codex, Claude | Repo analysis and PR prep. | Workflow, scripts | Active | Medium |
```

Keep descriptions factual and compact.

## Evaluation Score

Every submission should be scored before it is added. Stars are only a weak signal; reviewers should prioritize whether the skill helps an agent complete a real task safely and repeatably.

| Area | Points | Review focus |
|---|---:|---|
| Task clarity | 0-2 | Clear real-world use case, inputs, outputs, and target user. |
| Reusable structure | 0-2 | More than a prompt: skill files, workflows, templates, scripts, examples, or references. |
| Platform and tool fit | 0-2 | Clear support for Codex, Claude, ChatGPT, Cursor, Copilot, MCP, n8n, CLI, browser, API, or local app workflows. |
| Validation and examples | 0-2 | Demo, tests, sample usage, CI checks, schema, or step-by-step verification. |
| Maintenance and safety | 0-2 | Recent activity, license clarity, safe defaults, confirmation rules, and credential/privacy guidance. |

Inclusion guide:

- 8-10: recommended.
- 6-7: acceptable with caveats.
- 4-5: use with care or re-review.
- Below 4: remove or do not include.

## Status Guide

- Active: recent commit, release, issue reply, or PR activity.
- Stable: slower updates, but still useful and not archived.
- Use with care: useful but sensitive, risky, or requiring extra review.

## Risk Guide

- Low: mostly read-only or content generation.
- Medium: modifies files, calls APIs, uses accounts, automates browsers, or syncs external systems.
- High: production changes, deletion, security testing, trading, payments, sensitive credentials, privileged accounts, or bulk external actions.

## PR Checklist

- [ ] Link points to the canonical repository.
- [ ] The project is not just a prompt dump.
- [ ] Evaluation score is at least 6, or the PR explains why a lower-scoring skill is still worth tracking.
- [ ] Platform, use case, includes, status, and risk are filled.
- [ ] Safety caveats are included for sensitive workflows.
- [ ] Link check passes.
