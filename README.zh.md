# ZeroPlot

> **Plot anything. From zero.**

ZeroPlot 是一个 Agent Skill：把意图、数据或参考素材变成可编辑视觉产物。

## 范围

从科研图起步，覆盖完整视觉栈：

```text
图表 → 图解 → 插图 → 海报 → Slides
```

输入可以是自然语言、数据集、代码、草图、截图、论文、网表、结构化规范或现有视觉。

输出优先保持可编辑：

- SVG、draw.io、Mermaid、TikZ、matplotlib 源码或结构化 JSON；
- PPTX 等结构化 Slides；
- PDF、PNG 交付文件；
- 没有可编辑路径时才使用纯位图。

## 核心定义

`plot` 指组织视觉元素，不只指统计绘图。

科研图是第一个验证场，不是产品边界。

## 安装

```bash
npx skills add blackblue-labs/zeroplot -g -a codex -y
```

Skill 位于 [`skills/zeroplot`](skills/zeroplot)。

## License

MIT。
