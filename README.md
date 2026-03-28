# AI Agents

108 specialized agents for Claude Code. Built through extensive research (Oparin n=600 evaluation, scientific literature on LLM prompting, A/B testing with 6 agent variants) and manual quality review of every agent file.

## Quick Start

1. **Copy files**: Put `.claude/` folder into your Claude Code working directory
2. **Add instructions**: Copy `CLAUDE.md` contents into your project's instruction file
3. **Done**: Claude automatically selects the right agent for each task

## Design Philosophy

Each agent is crafted based on research-proven principles:

- **Domain checklists** over generic advice — specific failure patterns the model might miss
- **Decision tables** encoding when to choose what — prevents wrong technology/pattern choices
- **Anti-patterns** preventing known failures — directly addresses common precision problems
- **Knowledge activation triggers** — section headers that activate the model's latent expertise
- **No rigid output templates** — proven #1 score killer in evaluations
- **No adjective lists** — zero measured lift over bare model
- **Conservative enhancement** of domain knowledge — the winning approach in n=600 evaluation

## Agent Categories

| Category | Count | Examples |
|----------|-------|----------|
| Development | 30+ | python-pro, typescript-pro, react-pro, golang-pro, rust-pro |
| DevOps & Infra | 15+ | kubernetes-architect, terraform-pro, cloud-architect, devops-engineer |
| Data & ML/AI | 10+ | data-scientist, ml-engineer, llm-architect, ai-engineer |
| Security & QA | 15+ | security-reviewer, penetration-tester, code-reviewer, tdd-guide |
| Architecture | 10+ | microservices-architect, api-designer, database-architect, event-sourcing-architect |
| Business & Design | 10+ | product-manager, ui-designer, ux-designer, prompt-engineer |
| Operations | 10+ | sre-engineer, observability-engineer, incident-responder, performance-engineer |

<details>
<summary>Full list of 108 agents</summary>

agent-organizer, ai-engineer, api-designer, api-documenter, backend-architect, backend-security-coder, bash-pro, build-engineer, build-error-resolver, c-pro, cli-developer, cloud-architect, code-reviewer, cpp-pro, csharp-pro, data-engineer, data-researcher, data-scientist, database-architect, database-optimizer, database-reviewer, debugger, dependency-manager, deployment-engineer, design-system-architect, devops-engineer, devops-incident-responder, devops-troubleshooter, django-pro, doc-updater, docs-architect, documentation-pro, dotnet-core-pro, dotnet-framework-pro, dx-optimizer, e2e-runner, electron-pro, elixir-pro, event-sourcing-architect, fastapi-pro, flutter-pro, frontend-developer, frontend-security-coder, full-stack-developer, go-build-resolver, go-reviewer, golang-pro, graphql-architect, haskell-pro, hybrid-cloud-architect, incident-responder, ios-pro, java-pro, javascript-pro, julia-pro, kotlin-pro, kubernetes-architect, legacy-modernizer, llm-architect, mcp-developer, mermaid-pro, microservices-architect, ml-engineer, mlops-engineer, mobile-developer, mobile-security-coder, monorepo-architect, network-engineer, nextjs-pro, observability-engineer, penetration-tester, performance-engineer, php-pro, planner, platform-engineer, posix-shell-pro, postgres-pro, product-manager, prompt-engineer, python-pro, python-reviewer, qa-pro, rails-pro, react-pro, refactor-cleaner, research-analyst, ruby-pro, rust-pro, scala-pro, security-reviewer, service-mesh-pro, spring-boot-pro, sql-pro, sre-engineer, swift-pro, tdd-guide, technical-writer, terraform-pro, test-automator, threat-modeling-pro, tutorial-engineer, typescript-pro, ui-designer, ux-designer, vector-database-engineer, vue-pro, websocket-engineer, wordpress-master

</details>

## Sources & Methodology

Agents were built by analyzing multiple sources and selecting the best content from each:

- **Original v1 agents** — hand-crafted domain knowledge preserved where valuable
- **Improved versions** — decision tables, anti-patterns, and domain checklists added
- **Oparin agent research** (n=600 evaluation) — methodology and structure validated
- **External collections** (augmnt, affaan-m, others) — cross-checked for unique domain content
- **Scientific research** — U-shaped attention (Liu et al.), instruction scaling (Distyl AI), terminal reinforcement (Google Research)

Every agent was manually reviewed with full reads of all available sources. No automated batch processing.

## Features

- **108 Specialized Agents**: Development, DevOps, security, data science, ML/AI, architecture, business
- **Research-Optimized**: Structure validated against n=600 evaluation data
- **Decision Tables**: Every agent encodes when-to-choose-what guidance
- **Anti-Patterns**: Prevent known failure modes specific to each domain
- **In-Session Loading**: Designed for direct context injection, not subprocess spawning
- **Zero Dependencies**: Pure markdown files

## License

MIT
