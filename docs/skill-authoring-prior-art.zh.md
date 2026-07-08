# Skill Authoring Prior Art

日期：2026-07-08

## 结论

Paper Skills 不应该直接做一个大而全的学术 workflow clone。更好的路线：

```text
superpowers 的纪律性
+ nature-skills 的 router / static / references 分层
+ Awesome-Journal-Skills 的 venue-pack 覆盖方式
+ science-skills 的 tool + reference + provenance 结构
+ Paper Skills 自己的 discipline-aware plot
```

先 copy 结构，不急着 copy 内容。内容复制只从 license 兼容项目开始，并保留上游署名。

## 可借鉴项目

| 项目 | License | 可借鉴点 | Copy 策略 |
| --- | --- | --- | --- |
| [`Yuan1z0825/nature-skills`](https://github.com/Yuan1z0825/nature-skills) | Apache-2.0 | `router + manifest + static/core + references + scripts`；中文用户模式；Nature/CNS 叙事能力 | 可 copy/adapt 结构和兼容片段，保留 Apache-2.0 署名和 NOTICE |
| [`google-deepmind/science-skills`](https://github.com/google-deepmind/science-skills) | Apache-2.0 | 每个科学数据库一个 skill；工具安装前置 skill；`SKILL_LICENSES.md` | 可 copy/adapt 结构；适合做可执行科研工具层 |
| [`Orchestra-Research/AI-Research-SKILLs`](https://github.com/Orchestra-Research/AI-Research-SKILLs) | MIT | 大目录 taxonomy；research lifecycle；paper-writing / research-ideation 分类 | 可 copy/adapt 轻量结构；避免照搬 autonomous research 大叙事 |
| [`Galaxy-Dawn/claude-scholar`](https://github.com/Galaxy-Dawn/claude-scholar) | MIT | 跨 coding / experiment / writing / publication 的 scholar platform 感 | 可参考产品结构；具体技能要逐项筛 |
| [`brycewang-stanford/Awesome-Journal-Skills`](https://github.com/brycewang-stanford/Awesome-Journal-Skills) | MIT | venue pack 规模化；official-source discipline；“router first, journal second” | 可 copy/adapt pack 骨架；适合先做 CS / engineering / circuits |
| [`Boom5426/Nature-Paper-Skills`](https://github.com/Boom5426/Nature-Paper-Skills) | MIT | Nature-style manuscript lifecycle；ATTRIBUTION 独立文件 | 可参考 attribution 和 lifecycle 分层 |
| [`jaechang-hits/SciAgent-Skills`](https://github.com/jaechang-hits/SciAgent-Skills) | CC BY 4.0 | bio / life-science 深域 skill registry；测试和模板目录 | 可 copy/adapt，但必须明确 CC BY attribution |
| [`Imbad0202/academic-research-skills`](https://github.com/Imbad0202/academic-research-skills) | CC BY-NC 4.0 | 完整 research -> write -> review -> revise -> finalize 平台化 | 不 copy 到 MIT repo；只 reference / adapter / idea-level 借鉴 |

## Superpowers 模式

Superpowers 的格式很值得直接借：

- bundle root 有 `README.md`、`LICENSE`、`.codex-plugin/plugin.json`、`assets/`、`skills/`。
- 每个 skill 是一个独立目录，顶层 `SKILL.md` 是唯一入口。
- 同目录放少量 supporting files，例如 `*-prompt.md`、`testing-anti-patterns.md`、`find-polluter.sh`。
- `agents/openai.yaml` 只放 UI 元数据：`display_name`、`short_description`。
- 只有重资料才进 `references/`、`examples/`、`scripts/`。
- flowchart 用 fenced `dot` block，配合 `render-graphs.js` 渲染。

Superpowers 的质量纪律也要借：

- `description` 只写触发条件，不写 workflow 摘要，避免 agent 只读描述就跳过正文。
- skill 是过程文档的 TDD：先观察不带 skill 的失败，再写最小规则，再用压力场景验证。
- 好 skill 有明确 “Iron Law / Red Flags / Common Rationalizations”，适合约束 agent 容易偷懒的行为。
- 不为普通参考资料强上 TDD。核心纪律 skill 要 TDD；普通 adapter / venue card 用 lighter review 即可。

Paper Skills 应采用“两层规约”：

1. 普通 skill：遵守本仓库轻量 schema。
2. 核心高风险 skill：再套 superpowers-style pressure test。

## 推荐 Paper Skills Schema

每个 skill pack 默认用 superpowers 风格：

```text
skills/<area>/
  SKILL.md                 # agent 入口；短 router；description 只写触发
  agents/openai.yaml        # UI 元数据
  README.md                # 人类说明；demo prompt；状态
  *-prompt.md              # 可选；subagent/reviewer prompt
  references/              # 可选；重材料
  scripts/                 # 可选；可执行工具
  examples/                # 可选；长例子
```

`SKILL.md` 建议固定为：

```text
frontmatter:
  name
  description: Use when ... 只写触发条件

body:
  Core Stance
  Routing
  Required Reads
  Workflow Contract
  Output Contract
  Source / License Rules
  Common Failures
```

## Copy 规则

- MIT / Apache-2.0：可以 copy/adapt，但要保留 license、署名、修改说明。
- CC BY 4.0：可以 copy/adapt，包括商用，但必须 attribution，且标明修改。
- CC BY-NC 4.0：不 copy 到 MIT repo；会污染商业使用。只做 reference / adapter。
- 未确认 license：不 copy。
- 官方网页规则：只写稳定原则；实时 deadline、page limit、APC、chair、impact factor 不写死。

## 最先该做的 3 件事

1. 新建 `docs/paper-skills-skill-schema.zh.md`：把上面 schema 变成项目规范。
2. 把 `skills/plot/SKILL.md` 升级成 router：`static/core` + `domains/*/references`。
3. 先做两个可展示 pack：
   - `plot/domains/integrated-circuits`
   - `venue-packs/computer-science`

先让一个垂直切片跑通：用户给论文段落 / 草图 / venue，agent 产出 figure spec、rubric、修改建议和可编辑产物。
