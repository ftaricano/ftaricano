# Fernando Taricano

Building agentic AI for SMB ops. Shipping production multi-agent systems on Claude Code + Codex. Operator at Grupo CPZ (Brazilian insurance brokerage holding). Available for advisory.

→ Twitter: [@taricanof](https://x.com/taricanof)

## What I do

I run a non-tech Brazilian SMB where production AI agents handle daily back-office: ETL across dozens of insurance carriers, financial pipelines, mailbox triage, operational reporting. The system runs on **Claude Code** (architecture, frontend), **Codex** (implementation ), and **Hermes** (productivity, research) — orchestrated by ~40 written ADRs.

In parallel, I ship and maintain open-source Model Context Protocol (MCP) servers as the infrastructure that makes the above work.

## Open-source MCP servers

Production-grade MCP servers for operator stacks:

- **[`mcp-onedrive-sharepoint`](https://github.com/ftaricano/mcp-onedrive-sharepoint)** ⭐6 — Microsoft Graph: OneDrive + SharePoint, 33 tools, device-code auth, also `ods` CLI
- **[`mcp-outlook`](https://github.com/ftaricano/mcp-outlook)** ⭐1 — Outlook / Exchange via MS Graph, 40 tools, 178 passing tests
- **[`mcp-whatsapp`](https://github.com/ftaricano/mcp-whatsapp)** ⭐2 — WhatsApp via Baileys (QR pairing, rate limited, circuit breaker, pt-BR templates)
- **[`mcp-server-trello`](https://github.com/ftaricano/mcp-server-trello)** — Trello, 23 tools, 93 unit tests
- **[`mcp-gmail-calendar`](https://github.com/ftaricano/mcp-gmail-calendar)** — Gmail + Calendar, 35 tools, OAuth multi-account
- **[`mcp-hub`](https://github.com/ftaricano/mcp-hub)** — MCP aggregation gateway behind one tool surface

## Architecture principles I ship by

- **Read-after-write** is default — agent self-report doesn't close a task
- **Source-of-truth design** — CRM wins even when empty so pending cases stay visible
- **Fail-closed before fail-open** — pipeline halts when upstream signal is unavailable
- **OAuth-only auth** — no paid API keys in production
- **Governance by ADR** — material decisions go to a written record, not chat history

## What I'm interested in

Production agentic AI in non-tech regulated SMBs. The boring auditable closure of a workflow: pull data, validate, publish, log, fail in a known way, notify a human only when intervention is genuinely needed.

Available for **advisory** and **fractional** engagements. DMs open on [Twitter](https://x.com/taricanof).

## Note

Business systems for Grupo CPZ (Competenza, Interpar, SegDigital, Ferga) live in private repos. What's public here is the infrastructure tooling I'd want regardless of the operator job.
