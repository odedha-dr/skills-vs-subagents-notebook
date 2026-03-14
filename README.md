---
status: active
lead: Oded Har-Tal
people: [Oded Har-Tal]
created: 2026-03-10
---

# Skills vs Sub-Agents: An Interactive Exploration

A Jupyter notebook that walks through the two fundamental patterns for extending AI coding assistants — skills (context injection) and sub-agents (context isolation) — with live API calls, conversation traces, and inline visualizations.

## Quick Start

```bash
cp .env.example .env   # add your ANTHROPIC_API_KEY
uv sync
uv run jupyter notebook notebook.ipynb
```

The notebook ships with pre-recorded outputs. Re-run cells to reproduce with your own API key.

## What's Included

The project is fully self-contained. The `src/` directory contains a bundled sample codebase (from the MCP benchmark project) that the notebook's agent loops explore during experiments. No external dependencies beyond an Anthropic API key are needed.
