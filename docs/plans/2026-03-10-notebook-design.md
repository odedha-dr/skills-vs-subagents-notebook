# Skills vs Sub-Agents Notebook — Design Doc

**Date:** 2026-03-10
**Status:** Approved

## Goal

A single Jupyter notebook that teaches the skill vs sub-agent patterns through live API calls, conversation traces, and inline visualizations. Audience: developers familiar with LLM APIs.

## Notebook Structure

| Cell | Type | Content |
|------|------|---------|
| 1 | Markdown | The Two Patterns — what skills and sub-agents are, with diagram |
| 2 | Code | Setup — imports, API client, helpers, tool definitions |
| 3 | Markdown | Pattern 1: Skill — explain context injection |
| 4 | Code | Run simple task as skill, print conversation trace |
| 5 | Markdown | Pattern 2: Sub-Agent — explain context isolation |
| 6 | Code | Run same task as sub-agent, print parent + child traces |
| 7 | Code | Side-by-side token chart for simple task |
| 8 | Markdown | Scaling Up — what happens with complex tasks? |
| 9 | Code | Run composed workflow as both patterns |
| 10 | Code | Token chart showing crossover |
| 11 | Markdown | Context Pollution — the hidden cost |
| 12 | Code | Visualize parent context size comparison |
| 13 | Markdown | When to Use Which — decision table + takeaways |

## Key Decisions

- Two tasks only: T1 (simple) and T4 (composed) — tell the full story
- All logic in notebook cells, no separate src/ package
- Pre-recorded outputs shipped, but cells are re-runnable with API key
- Charts via matplotlib inline
