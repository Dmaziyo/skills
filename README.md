# Agent Skills

[中文版](./README.zh-CN.md) | [English](./README.md)

A collection of agent skills that extend capabilities across planning, development, and tooling.

## Install all skills (one command)

Use the official [`skills` CLI](https://github.com/vercel-labs/skills) (`npm` package `skills`) to install every skill in this repository at once:

```bash
npx skills@latest add Dmaziyo/skills --all -y
```

- **Preview** what would be installed (no install): `npx skills@latest add Dmaziyo/skills --list`
- **From a local clone** of this repo (run at the repository root): `npx skills@latest add . --all -y`
- **Equivalent** to `--all`: `--skill '*'` (you can add `-a <agent>` to target a specific agent)
- Install globally (`-g`) or copy instead of symlink (`--copy`) as needed; see `npx skills@latest add --help`.

## Development Quality

These skills help keep implementation clean, explicit, and maintainable.

### create-plan

Creates detailed implementation plans through an interactive and iterative workflow, focusing on analysis, options, phased structure, and explicit validation criteria before coding.

`npx skills@latest add Dmaziyo/skills/create-plan`

### code-simplifier

Simplifies and refines code for clarity, consistency, and maintainability while preserving all functionality. Focuses on recently modified code unless instructed otherwise.

`npx skills@latest add Dmaziyo/skills/code-simplifier`

### grill-me

Continuously challenges a proposal or design through focused questioning until there is shared understanding, while resolving each branch of the decision tree and its dependencies.

`npx skills@latest add Dmaziyo/skills/grill-me`

### research

Researches and documents the codebase for a specific topic using a strict parallel sub-agent workflow, producing a structured technical map of what currently exists.

`npx skills@latest add Dmaziyo/skills/research`

## Repository Layout

- [create-plan/SKILL.md](./create-plan/SKILL.md)
- [code-simplifier/SKILL.md](./code-simplifier/SKILL.md)
- [grill-me/SKILL.md](./grill-me/SKILL.md)
- [research/SKILL.md](./research/SKILL.md)
