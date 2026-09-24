# Fernando Taricano

Applied AI engineer. I build and run production agent systems on Claude Code, Codex and MCP.

At Grupo CPZ, a Brazilian insurance brokerage with no engineering team, I moved the back-office from spreadsheets and email onto pipelines and agents I built and operate every day.

→ X: [@taricanof](https://x.com/taricanof) · [LinkedIn](https://www.linkedin.com/in/fernando-taricano-a1388415b)

## What I build

An operating layer for agents, not a pair of chatbots: domain workspaces, a skill library, written rules and one delivery contract every agent follows. It is wired into the systems the operation already uses: Microsoft 365, the policy-admin system, the CRM, Power BI. Work is routed across Claude Code, Codex and other harnesses depending on the task.

The integration layer is open source. Each repo has CI and tests, and each one is used in production.

## Open-source MCP servers & CLIs

- **[`mcp-outlook`](https://github.com/ftaricano/mcp-outlook)** — Outlook / Exchange via Microsoft Graph. 40 tools, CLI, large-attachment flows that stay under MCP token limits.
- **[`mcp-onedrive-sharepoint`](https://github.com/ftaricano/mcp-onedrive-sharepoint)** — OneDrive + SharePoint via Microsoft Graph. Safe core profile by default, opt-in full profile, also usable as the `ods` CLI.
- **[`mcp-slack`](https://github.com/ftaricano/mcp-slack)** — Slack with OAuth, typed errors, retry/backoff, safe file uploads and a CLI. 37 tools.
- **[`telegram-claude-code-bridge`](https://github.com/ftaricano/telegram-claude-code-bridge)** — Claude Code over Telegram: one session per forum topic, durable delivery, OAuth/CLI-only. Independent fork, evolved.
- **[`mcp-server-trello`](https://github.com/ftaricano/mcp-server-trello)** — Trello, 31 tools, `trello` CLI, 152 unit tests. Started as a fork of delorenj/mcp-server-trello.
- **[`gws`](https://github.com/ftaricano/mcp-gmail-calendar)** — Google Workspace, CLI-first (Gmail, Calendar, Drive, Docs, Sheets); MCP is the adapter. Beta.

## Principles I ship by

- **Execution ≠ effect.** "It ran" is not "it worked"; read the result back.
- **Fail closed.** Missing upstream data stops the pipeline instead of producing quiet, wrong output.
- **Source of truth wins, even when empty.** Pending cases stay visible.
- **Least privilege.** OAuth where possible; credentials live in a vault, never in the repo.
- **Decisions in writing.** Material changes go to a written record, not a chat log.

## Interested in

Production agentic AI in non-tech, regulated businesses: the boring, auditable closure of a workflow. Pull data, validate, publish, log, fail in a known way, and call a human only when it matters.

Business systems for Grupo CPZ live in private repos.
