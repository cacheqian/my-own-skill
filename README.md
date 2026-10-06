# My Own Skills

可复用的 Agent skills。

## notion-page-design

[查看完整 Skill](notion-page-design/SKILL.md)

用于创建、重写、美化和维护 Notion 原生页面，适合技术解读、论文介绍、研究报告、方案比较与项目文档。支持读者导向的内容结构、分栏、Callout、表格、折叠、来源核验，以及保留原图并补充可编辑 Mermaid。

### 目录

```text
notion-page-design/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── page-patterns.md
    ├── content-and-sources.md
    ├── diagrams-and-media.md
    ├── data-and-views.md
    ├── operations-and-validation.md
    └── native-blocks.md
```

### 使用

将整个 `notion-page-design` 目录放入所用 Agent 的 skills 目录，保留 `agents/` 和 `references/`。在任务中指定使用 `notion-page-design`，并提供目标 Notion 页面与需要参考的资料。操作 Notion 页面时，需要环境中提供可用的 Notion 连接器或 API 及相应页面权限。
