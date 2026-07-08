# Paper Skills Skill Schema

日期：2026-07-08

## 原则

Paper Skills 的 skill 要服务非 CS 科研用户。skill 不是长文章，而是 agent 执行科研任务时的规约。

核心原则：

- `description` 只写触发条件，不写完整流程。
- `SKILL.md` 做 router；重知识放 `references/`。
- 复制外部内容前先查 license；默认 adapter / reference 优先。
- 学科差异优先：写作、图、引用、审稿标准都要按领域分化。
- 可执行检查优先：能用脚本验证的，不靠文字提醒。

## 目录模板

```text
skills/<area>/
  SKILL.md
  README.md
  references/
  templates/
  scripts/
  domains/
  venues/
```

按需创建目录。不要为了整齐创建空目录。

## SKILL.md 模板

```md
---
name: <skill-name>
description: >-
  Use when <trigger symptoms, user intents, task contexts>. Include Chinese and
  English trigger phrases when useful. Do not summarize workflow here.
---

# <Skill Name>

## Core Stance

One or two sentences. Say what must be protected.

## Routing

Map user task to domain / venue / workflow. Load only matching references.

## Required Reads

- Always read: small core files.
- Read on demand: heavy references, official-source maps, templates.

## Workflow Contract

Before output, identify:

- domain / venue;
- input materials;
- target artifact;
- must-preserve claims / entities;
- hard-fail criteria;
- verification plan.

## Output Contract

State exact output shape: table, figure spec, rebuttal draft, checklist, file path.

## License / Source Rules

Never copy upstream content without compatible license and attribution.

## Common Failures

List failures that make output unusable.
```

## README.md 模板

Human-facing. Include:

- what this skill area covers;
- current state;
- demo prompt;
- integration bias;
- known limits.

## Reference 文件

Use references for durable, high-token content:

- official-source maps;
- venue / domain rubrics;
- paper structure rules;
- figure grammar;
- citation norms;
- benchmark cases.

Keep volatile facts out unless they point to live official pages.

## Copy / Adapt Checklist

- [ ] Source project and exact path recorded.
- [ ] License compatible with MIT repo.
- [ ] Attribution added.
- [ ] Modified content marked if required.
- [ ] No raw tokens, API keys, or personal data.
- [ ] Official source wins over copied skill text.

## Test Level

| Skill Type | Validation |
| --- | --- |
| lightweight adapter | read-through + one demo prompt |
| venue / domain pack | one realistic manuscript scenario |
| core discipline skill | superpowers-style pressure test |
| script-backed skill | run script on sample input |

## Naming

- folder: kebab-case;
- broad skill: verb or noun area, e.g. `writing`, `review`, `plot`;
- domain pack: stable field name, e.g. `integrated-circuits`;
- venue pack: official venue family or normalized venue name.
