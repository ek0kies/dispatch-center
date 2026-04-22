# Dispatch

Local-first control plane for agent automation.

Dispatch is not a multi-agent framework or workflow designer.
It is built for running, scheduling, observing, and controlling agent automations on a single machine.

## Positioning

Dispatch focuses on five things:

- automation
- scheduling
- queue visibility
- operator control
- result assets

Dispatch does not focus on:

- generic multi-agent orchestration
- graph workflow design
- enterprise RBAC and approval chains
- cloud-first infrastructure

## Product Shape

Core objects:

- Agent
- Automation
- Schedule
- Dispatch Queue
- Run
- Result Asset
- Policy
- Cost Ledger

Default runtime direction:

- local-first
- SQLite as embedded state store
- file-based definitions
- file-based result artifacts
- visible dispatch control plane

## Principles

- Zero external infrastructure by default
- One command to start
- Files for definitions, SQLite for runtime truth
- Clear state transitions over hidden magic
- Operator-friendly controls over opaque autonomy

## Repo Scope

This repository is the new clean-line for Dispatch.

Current work here is focused on:

1. replacing PostgreSQL and Redis defaults with a local-first runtime
2. rebuilding the scheduling kernel around SQLite
3. turning the current agent visualization direction into a real dispatch center
4. making the community edition easy to install, demo, and share on GitHub

## Repository Layout

- `src/`: runtime and control plane code
- `examples/`: killer templates
- `assets/`: screenshots and demo materials

## Status

Early rebuild.

The repository is being reset around a local-first architecture before implementation starts.
