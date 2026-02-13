# AI Agents

109 specialized agents for Claude Code. Curated from 4 sources: affaan-m, lst97, wshobson, and supatest. Cleaned up and optimized for in-session loading.

## Quick Start

1. **Copy files**: Put `.claude/` folder into your Claude Code working directory
2. **Add instructions**: Copy `CLAUDE.md` contents into your project's instruction file
3. **Done**: Claude automatically selects the right agent for each task

## Why This Fork?

Default Claude Code spawns agents as separate subprocesses with isolated memory. This wastes tokens and produces poor results.

**This fork loads agents directly into the main session context.** Benefits:
- Agents share memory and research results
- Much lower token usage
- Significantly better output quality

Combine with [web_search_agent](https://github.com/anthropics/web_search_agent) for even better research capabilities.

## Features

- **115 Specialized Agents**: Development, DevOps, security, data science, ML/AI, business
- **Automatic Selection**: Claude picks the right agent for each subtask
- **In-Session Loading**: No subprocesses, shared context
- **Zero Dependencies**: Pure markdown files

## Agent Categories

| Category | Count | Examples |
|----------|-------|----------|
| Development | 30+ | python-pro, typescript-pro, react-pro, golang-pro |
| DevOps & Infra | 15+ | kubernetes-specialist, terraform-specialist, cloud-architect |
| Data & ML/AI | 10+ | data-scientist, ml-engineer, llm-architect |
| Security & QA | 15+ | security-reviewer, penetration-tester, code-reviewer |
| Architecture | 10+ | microservices-architect, api-designer, database-optimizer |
| Business & Design | 15+ | product-manager, ui-designer, ux-designer |
| Debugging | 10+ | debugger, performance-engineer, incident-responder |

<details>
<summary>Full list of 109 agents</summary>

accessibility-tester, agent-organizer, ai-engineer, angular-architect, api-designer, api-documenter, architect, backend-architect, build-error-resolver, cli-developer, cloud-architect, code-reviewer, database-reviewer, debugger, deployment-engineer, devops-engineer, devops-incident-responder, devops-troubleshooter, diagnostic-command-generator, diagnostics-gui, directus-specialist, discovery-helper, discovery-suggester, doc-updater, documentation-expert, dotnet-core-expert, dotnet-framework-4.8-expert, dx-optimizer, e2e-runner, electron-pro, embedded-systems, event-sourcing-architect, frontend-developer, full-stack-developer, golang-pro, go-build-resolver, go-reviewer, graphql-architect, hybrid-cloud-architect, incident-responder, java-architect, java-pro, javascript-pro, julia-pro, kotlin-expert, kubernetes-architect, legacy-modernizer, llm-architect, logger, master-control-gui, mermaid-expert, microservices-architect, mobile-developer, mlops-engineer, monorepo-architect, network-engineer, nextjs-pro, nlp-engineer, nx-console-gui, offline-mode-implmentor, performance-engineer, php-pro, planner, platform-engineer, playwright-test-architect, playwright-test-automater, playwright-test-data-manager, playwright-test-executor, playwright-test-framework, playwright-test-orchestrator, plugin-installer, plugin-manager, plugin-marketplace, plugin-updater, postgres-pro, prod-mode-implmentor, product-manager, project-manager, prompt-engineer, pro-plugins-installer, pro-plugins-marketplace, pro-plugins-updater, pro-updater, python-pro, python-reviewer, qa-expert, quick-run-gui, rails-expert, react-pro, refactor-cleaner, refactoring-specialist, release-note-architect, release-note-generator, rust-pro, scala-pro, script-to-plugin-migrater, security-auditor, security-reviewer, service-mesh-expert, shell-helpers-guide, spring-boot-expert, sql-pro, sre-engineer, swift-expert, tdd-guide, terraform-specialist, test-automator, tracer, tracer-ui, typescript-pro, ui-designer, ux-designer, vector-database-engineer, vue-specialist

</details>

## License

MIT
