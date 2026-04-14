# Agent Skills

[中文版](./README.zh-CN.md) | [English](./README.md)

一个用于扩展智能体在规划、开发与工具使用能力的技能集合。

## 一键安装全部技能

使用官方 [`skills` CLI](https://github.com/vercel-labs/skills)（npm 包 `skills`）可一次性安装本仓库中所有技能：

```bash
npx skills@latest add Dmaziyo/skills --all -y
```

- **仅列出**可发现技能、不安装：`npx skills@latest add Dmaziyo/skills --list`
- **本地克隆**本仓库后，在仓库根目录执行：`npx skills@latest add . --all -y`
- **与 `--all` 等价**的写法：`--skill '*'`（可按需加 `-a <agent>` 指定智能体）
- 需要时可加 `-g`（全局）、`--copy`（复制而非符号链接）等，详见 `npx skills@latest add --help`。

## 开发质量

这些技能用于让实现保持清晰、显式且易维护。

### create-plan

通过交互式、迭代式流程创建详细实施计划，重点覆盖现状分析、方案对比、分阶段结构与编码前验证标准。

`npx skills@latest add Dmaziyo/skills/create-plan`

### code-simplifier

在不改变任何功能的前提下，简化并优化代码的清晰度、一致性与可维护性。默认聚焦于最近修改过的代码，除非另有说明。

`npx skills@latest add Dmaziyo/skills/code-simplifier`

### grill-me

围绕一个方案或设计持续追问，直到形成共同理解，并沿着设计决策树逐一解决各分支及其依赖关系。

`npx skills@latest add Dmaziyo/skills/grill-me`

### research

通过严格的并行子代理工作流，对指定主题进行代码库调研与文档化，产出“当前实现现状”的结构化技术地图。

`npx skills@latest add Dmaziyo/skills/research`

## 仓库结构

- [create-plan/SKILL.md](./create-plan/SKILL.md)
- [code-simplifier/SKILL.md](./code-simplifier/SKILL.md)
- [grill-me/SKILL.md](./grill-me/SKILL.md)
- [research/SKILL.md](./research/SKILL.md)
