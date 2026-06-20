# AI Agents

111 specialized AI agents for [Claude Code](https://claude.ai/download). Each agent is a domain expert — loaded on demand as a Markdown file, applied to the current task, then discarded. No subprocesses, no configuration, no dependencies.

## Why use it

Generic AI assistants produce mediocre results on specialized work. A domain-specific agent with checklists, anti-patterns, and decision tables produces measurably better output — validated in n=600 evaluations.

- **PostgreSQL migration?** Load `postgres-pro` — it knows indexing strategies, migration patterns, and when to use BRIN vs B-tree.
- **SwiftUI refactor?** Load `swift-pro` — it understands actor isolation, `@MainActor` rules, and iOS lifecycle pitfalls.
- **Security audit?** Load `security-reviewer` — OWASP Top 10, injection vectors, auth bypass patterns.

## Agent Quality — Real-Project Tested

All 111 agents have been tested and optimized through a rigorous methodology:

**Method:** Each agent was tested in a 3-way comparison (original / polished / smart-applied) on real production codebases — not synthetic tasks. Tested on real production codebases.

**Result:** The winning variant for each agent was selected based on objective criteria: finding accuracy, evidence quality, cross-file tracing depth, and zero false positives. Agents were compared head-to-head against Claude Code's own native subagents — **our agents won every comparison.**

**Cognitive Mode Tags:** Each agent in INDEX.md carries a Mode tag (TRACE / SWEEP / KNOW) derived from these tests, indicating which cognitive approach it's best at. This helps match the right agent to the task type.

- **TRACE** — best at following data/logic/flow through code (bug hunting, pipeline analysis)
- **SWEEP** — best at systematic checklist verification (security audits, idiom reviews)
- **KNOW** — best at applying deep domain/framework expertise (.NET, Spring, Django)

## Quick Start

```bash
git clone https://github.com/itohnobue/ai-agents-claude-code
cp -R ai-agents-claude-code/.claude /path/to/your/project/
cp ai-agents-claude-code/CLAUDE.md /path/to/your/project/
```

If you already have a `CLAUDE.md`, append this one instead of overwriting. Browse `.claude/agents/INDEX.md` for the full categorized directory.

## What's included

| Category | Count | Examples |
|----------|:-----:|----------|
| Language Implementation | 22 | python-pro, golang-pro, rust-pro, typescript-pro, cpp-pro |
| Web Frameworks | 10 | react-pro, nextjs-pro, django-pro, fastapi-pro, vue-pro |
| Architecture | 9 | backend-architect, api-designer, database-architect, microservices-architect |
| DevOps & Infrastructure | 11 | devops-engineer, kubernetes-architect, terraform-pro, sre-engineer |
| Security | 6 | security-reviewer, penetration-tester, threat-modeling-pro |
| Database | 5 | postgres-pro, sql-pro, database-optimizer |
| Testing & QA | 5 | code-reviewer, tdd-guide, test-automator, e2e-runner |
| AI & ML | 5 | ai-engineer, ml-engineer, prompt-engineer, llm-architect |
| Frontend & Mobile | 5 | frontend-developer, ios-pro, ui-designer, ux-designer |
| Documentation | 7 | documentation-pro, technical-writer, tutorial-engineer |
| Incident Response | 4 | incident-responder, debugger, devops-troubleshooter |
| Specialized | 19 | build-engineer, cli-developer, product-manager, research-analyst, legacy-modernizer |

Every agent includes domain-specific **checklists** (not generic advice), **anti-patterns** (known failure modes to avoid), and **decision tables** (when to choose what).

Full directory: `.claude/agents/INDEX.md`

## How agents are built

Structure validated against n=600 evaluations (Oparin research). Built through manual review of multiple agent collections, cross-checked for unique domain content. No automated batch processing. Pure Markdown — zero dependencies.

## License

MIT
