# Helx Systems

<div align="center">

<img src="assets/logo.svg" alt="Helx Systems Logo" width="120" height="120" />

### Deterministic Systems & Agentic Infrastructure

An open-source systems engineering collective focused on low-latency developer tooling, autonomous agent runtimes, and defensive infrastructure.

[Website](https://santiagopiedrahita.dev) • [Maintainer](https://github.com/TicoraX)

---

</div>

## Engineering Manifesto

Helx Systems adheres to three non-negotiable principles of software construction:

1. **Deterministic Execution over Heuristics**: Systems must run predictably. We reject brittle fallbacks and hidden side effects across toolchains and agent execution environments.
2. **Empirical Verification (Zero-Mock Socket Suites)**: Network, proxy, and process boundaries are tested directly against real operating system primitives. If it touches sockets or kernels, it is validated without mocks.
3. **Strict Context & Token Economics**: Agent workflows must respect hard boundaries. We engineer zero-cost abstractions, semantic context packaging, and surgical delegation to eradicate token waste and quota exhaustion.

---

## Core Ecosystem

### [StackHelx](https://github.com/TicoraX/StackHelx)
*Local Development Orchestrator & Native Model Context Protocol (MCP) Gateway*
- Asynchronous local proxy, reactive console, and native MCP server for autonomous agents.
- 474 unit and integration tests executing against real OS network sockets.
- Distributed via `uv tool` with multi-platform compatibility across Linux, macOS, and Windows.

### [OrqueHelx](https://github.com/TicoraX/OrqueHelx)
*Multi-Provider Agent Delegation & Quota Management Router*
- Systems-level delegation plugin for the Hermes agent runtime, routing subagent tasks across heterogeneous LLM subscriptions (Claude, Codex, Antigravity) and ACP CLIs (OpenCode).
- Runtime lifecycle interception via `pre_tool_call` and `api_request_error` hooks to eliminate unauthorized network egress.
- Persistent execution telemetry and state management backed by SQLite (`pausas.db`).

### [rtok](https://github.com/TicoraX/rtok)
*High-Performance Terminal Agent Studio & Context Optimizer*
- Terminal cabin developed in Rust applying The Elm Architecture (TEA/MVI) with Tokio async runtime for sub-16ms latency.
- Surgical context window packing engine managing 2k–8k token budgets through structured XML manifests.

### [EStiri Design System](https://github.com/TicoraX/skills)
*Canonical Technical Ledger Design System*
- Visual specification and design tokens: warm neutral paper ground, charcoal ink, terracotta interactive accents (`#bf4e28`), and IBM Plex typography.
- Eradicates artificial AI aesthetic patterns in favor of structured technical ledger grammar.

---

## Architecture & Tooling Standards

```
                     +---------------------------------------+
                     |         Helx Systems Ecosystem        |
                     +---------------------------------------+
                                         |
         +-------------------------------+-------------------------------+
         |                               |                               |
         v                               v                               v
   [ StackHelx ]                   [ OrqueHelx ]                      [ rtok ]
 Local Dev & Proxy              Agent Router & Quotas           Terminal & Context
  (Python / FastAPI)               (Python / SQLite)               (Rust / Tokio)
         |                               |                               |
         +-------------------------------+-------------------------------+
                                         |
                                         v
                            [ EStiri Design System ]
                        Technical Ledger Visual Language
```

---

## Maintainer & Governance

Helx Systems is founded and maintained by [Santiago Piedrahita Quintero](https://github.com/TicoraX). 

All software within this organization is published under permissive open-source licenses (MIT / Apache-2.0). Security disclosures should be submitted directly to `santiagohelxsystem@gmail.com`.
