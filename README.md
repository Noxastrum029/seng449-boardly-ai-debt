# SENG 449 – Boardly: Technical Debt in AI-Generated Code

Engineering Design II · Project 02 – Refactoring AI-Generated Code
Team: Berat Yılmaz (PM), Hüseyin Emir Macit

## Goal
Generate the same full-stack app (Boardly, a simple Trello-like task manager) from one spec using two models in Cursor (Claude and GPT), measure the technical debt, then refactor the backend while preserving behavior and compare before/after.

## Stack
TypeScript · Node.js/Express · Prisma/PostgreSQL · React · JWT

## Repository Structure
- `docs/spec.md` – single specification given to both models
- `docs/prompts/` – prompt log per model (reproducibility)
- `docs/reports/` – technical reports
- `apps/claude-baseline`, `apps/gpt-baseline` – AI-generated code (untouched, tagged `v0-ai-baseline-*`)
- `analysis/before`, `analysis/after` – metric outputs (SonarQube, ESLint, jscpd, dependency-cruiser, coverage)

## Workflow
- `[ai-gen]` commits: AI output only, no manual edits
- `[refactor]` commits: human refactoring on separate branches, merged via PR
- Behavior locked with tests before any refactoring

## Out of Scope
Vulnerability hunting, building a new review tool, frontend refactoring, energy measurement.
