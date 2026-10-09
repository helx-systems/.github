# Helx Systems

<img src="../assets/logo.svg" alt="Helx Systems logo" width="96" height="96" />

Helx is the name under which [Santiago Piedrahita Quintero](https://github.com/TicoraX) publishes
his developer tools. Each one started as a problem he had first, and each ships with tests you can
run.

## Tools

**[StackHelx](https://github.com/TicoraX/StackHelx)** — local dev environment orchestrator, on PyPI.
One file at the project root and `shx up` brings up ports, Docker, backend and frontend. Includes an
MCP server so agents can start and inspect services. 474 tests against real OS sockets, CI on Linux,
macOS and Windows.

**[OrqueHelx](https://github.com/TicoraX/OrqueHelx)** — Hermes Agent plugin for delegating work
between models on your own subscriptions (Claude, Codex, Antigravity, OpenCode). The model picks a
route per call; when a quota runs out, you decide where the task goes.

**[OptiHelx](https://github.com/TicoraX/OptiHelx)** — Windows maintenance suite with dry-run mode on
every destructive action.

**[LuckHelx](https://github.com/TicoraX/LuckHelx)** — local desktop app that turns daily tasks into
XP and rewards.

## How the tools are built

- Acceptance criteria are written before the code; nothing is called done without a passing test or
  a measurement.
- Code that touches sockets, processes or the file system is tested against the real OS, not mocks.
- Destructive actions get a dry-run first.

StackHelx, OrqueHelx and OptiHelx are MIT licensed. Contact: santiagohelxsystem@gmail.com
