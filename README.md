# SENG 449 – Boardly: Cleaning Up AI-Generated Code Safely

Engineering Design II · Project 02 – Refactoring AI-Generated Code
Team: Berat Yılmaz (PM), Hüseyin Emir Macit

## Goal
Generate the same full-stack app (Boardly) from one spec with two models in Cursor (Claude, GPT), measure its technical debt, and compare three refactoring strategies at equal effort: Manual, Unguided LLM, Guided LLM (test + metric feedback).

## Research Questions
- RQ1: What technical-debt profile do the two AI-generated codebases carry?
- RQ2: How well does each strategy preserve behavior?
- RQ3: How do the strategies differ in maintainability gain and effort?

## Stack and Tools
TypeScript · Express · Prisma/PostgreSQL · React · Jest · Supertest · StrykerJS · SonarCloud · ESLint · jscpd · dependency-cruiser · autocannon

## Repository Structure
- `docs/spec.md` – single specification
- `docs/prompts/` – prompt logs per model
- `docs/reports/` – technical reports
- `apps/claude-baseline`, `apps/gpt-baseline` – untouched AI output (tags `v0-ai-baseline-*`)
- `tests/acceptance/` – team-written acceptance tests (behavior reference)
- `analysis/before`, `analysis/after` – metric outputs

## Conventions
`[ai-gen]` commits = AI output only · `[refactor]` commits = one refactoring step each, via PR

## Out of Scope
Vulnerability hunting (P04), attack graphs (P03), new review tool (P06), frontend refactoring, energy measurement.
