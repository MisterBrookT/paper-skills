<div align="center">
  <img src="assets/paper-skills-icon.png" width="96" alt="Paper Skills 图标">
  <h1>Paper Skills</h1>
  <p><strong>领域特制的论文 AI skill 库。</strong></p>
  <p>
    写作、引用、审稿、返修、期刊规范和科研图，都由学科语境塑造。
  </p>
  <p>
    <a href="README.md">English</a>
  </p>
  <p>
    <a href="https://github.com/MisterBrookT/paper-skills/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/MisterBrookT/paper-skills?style=flat-square"></a>
    <a href="https://github.com/MisterBrookT/paper-skills"><img alt="Status" src="https://img.shields.io/badge/status-draft-8a6f3d?style=flat-square"></a>
    <a href="https://github.com/MisterBrookT/paper-skills"><img alt="Skills" src="https://img.shields.io/badge/skills-writing%20%7C%20citation%20%7C%20review%20%7C%20plot-1f2933?style=flat-square"></a>
    <a href="LICENSE"><img alt="License" src="https://img.shields.io/badge/license-MIT-lightgrey?style=flat-square"></a>
  </p>
</div>

![Paper Skills overview](assets/paper-skills-hero.jpg)

## 这是什么

Paper Skills 是一个 agent 可读的科研论文 skill 库，面向论文生产中的繁琐流程：起草、润色、引用、审稿回复、期刊规范和科研图。

核心判断：每个学科都有自己的论文表达语言。它不只包含英文句子，还包括证据组织、引用习惯、审稿标准、图形语法和期刊 taste。

## 技能区域

| 区域 | 覆盖内容 | 当前状态 |
| --- | --- | --- |
| `writing` | 润色、翻译、改写、论证修复。 | 架子 |
| `citation` | 文献检索、引用校验、参考文献审计和导出。 | 架子 |
| `review` | 审稿人模拟、返修信、修订 QA 和逐点回复。 | 架子 |
| `venue-packs` | 期刊、会议和学科特定规范。 | 架子 |
| `plot` | 学科特质化科研图和可编辑图形 skill。 | 种子案例 |

## 为什么做

学术 skill 包已经有不少优秀项目。Paper Skills 不应该从零重做所有写作、引用和返修流程。第一步是调研、致谢和整合已有工作。

当前第一块原创重点是 `plot`：不同学科的科研图应该有不同的领域包。材料图、医学图、交通图、集成电路图和计算机系统图，不应该套同一套通用流程图模板。

## `plot`：学科特质化科研图

第一批种子领域：

| 领域 | 路径 | 图形类型 |
| --- | --- | --- |
| 集成电路 | [`skills/plot/domains/integrated-circuits`](skills/plot/domains/integrated-circuits) | 模拟电路 schematic、开关电容图、电路架构图 |
| 计算机科学 | [`skills/plot/domains/computer-science`](skills/plot/domains/computer-science) | 系统图、模型结构图、pipeline、实验设置图 |

后续社区方向包括材料科学、医学和生物医学、交通与运输、生物学和金融。

## 贡献者

Paper Skills 按贡献者参与的领域和具体工作署名，不只统计 commit 数量。

| 贡献者 | Background | 领域 | 贡献 |
| --- | --- | --- | --- |
| [布布](https://github.com/MisterBrookT) | @KoinaAI · CS PhD @ ZJU | 计算机科学、科学可视化、AI agents | 发起人、项目方向、`plot` |

贡献了 skill、领域包、benchmark、审阅或整合？请在同一个 pull request 中把姓名、背景、领域和贡献加入此表。

## 目录

```text
skills/
  writing/
  citation/
  review/
  venue-packs/
  plot/
    domains/
      integrated-circuits/
      computer-science/
integrations/
  catalog.md
docs/
  academic-skill-pack-survey.md
registry.yaml
```

## 安装

目前还没有稳定安装方式。这个仓库仍是公开 scaffold。

现在可以在 agent 会话里直接引用对应的 `SKILL.md` 或 README。

## 整合原则

Paper Skills 会优先使用 adapter 和引用，而不是直接复制外部 skill。后续若复制或修改上游内容，必须遵守上游许可证并保留署名。

见 [ACKNOWLEDGEMENTS.md](ACKNOWLEDGEMENTS.md)。

## 本月路线

- 把 `plot` 的集成电路和计算机科学 demo 做具体。
- 把各 skill 的 demo 扩展成可复用 benchmark case。
- 继续扩展整合目录，补上署名说明和 adapter 计划。
- 随着整合推进，持续明确上游署名和贡献规则。
- 第一批 skill 可用后，再加稳定安装命令。

## Star History

<a href="https://www.star-history.com/?repos=MisterBrookT%2Fpaper-skills&type=date&legend=top-left">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=MisterBrookT/paper-skills&type=date&theme=dark&legend=top-left&sealed_token=Bl9TTZcLJ8xuZ2JiXJvdoqhqltSIwOV0kKxKUnRZ_VGoj2Az5wq06QZkHkCVYw4rQw_kAqO7f-nDVktPAUDcI_KAaTxewLISn-S4dzF_yZBnb9tuxFNd--xCx-wR5deSpfzUMllQqVAgbCdHnfjYBEm28rXHnzr_8ny-SFmxVbua99Xg1hNf0TzPVCrA" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=MisterBrookT/paper-skills&type=date&legend=top-left&sealed_token=Bl9TTZcLJ8xuZ2JiXJvdoqhqltSIwOV0kKxKUnRZ_VGoj2Az5wq06QZkHkCVYw4rQw_kAqO7f-nDVktPAUDcI_KAaTxewLISn-S4dzF_yZBnb9tuxFNd--xCx-wR5deSpfzUMllQqVAgbCdHnfjYBEm28rXHnzr_8ny-SFmxVbua99Xg1hNf0TzPVCrA" />
   <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=MisterBrookT/paper-skills&type=date&legend=top-left&sealed_token=Bl9TTZcLJ8xuZ2JiXJvdoqhqltSIwOV0kKxKUnRZ_VGoj2Az5wq06QZkHkCVYw4rQw_kAqO7f-nDVktPAUDcI_KAaTxewLISn-S4dzF_yZBnb9tuxFNd--xCx-wR5deSpfzUMllQqVAgbCdHnfjYBEm28rXHnzr_8ny-SFmxVbua99Xg1hNf0TzPVCrA" />
 </picture>
</a>

## License

MIT。外部 skill 的整合仍需单独检查上游许可证并保留署名。
