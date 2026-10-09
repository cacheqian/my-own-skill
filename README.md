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

## concise-writing

[查看完整 Skill](concise-writing/SKILL.md)

用于精简文章、文档、报告、方案和消息。先合并结构上的重复，再压缩句段，保留核心观点、必要论证、关键边界、引用与作者语气，不设固定压缩比例。

### 使用

将整个 `concise-writing` 目录放入所用 Agent 的 skills 目录，保留 `SKILL.md` 和 `agents/openai.yaml`。在任务中指定使用 `concise-writing`；支持对应语法的环境可用 `$concise-writing` 调用。也可直接提出“精简表述”“太啰嗦”“压缩篇幅”等请求。

## report-writing

[查看完整 Skill](report-writing/SKILL.md)

用于将原始材料改写为老板汇报、项目进展、能力建设、方案对比与阶段规划。文字提炼结论和判断，表格组织结构化信息，按需使用 1～2 张统一风格的关键画板；保留事实、数据口径、必要边界及用户指定结构。

### 目录

```text
report-writing/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── report-patterns.md
    └── style-reference.md
```

### 使用

将整个 `report-writing` 目录放入所用 Agent 的 skills 目录，保留 `agents/` 和 `references/`。在任务中指定使用 `report-writing`；支持对应语法的环境可用 `$report-writing` 调用。也可直接提供材料并提出“整理成汇报”或“按汇报风格改写”。基础改写不依赖访问样本文档；实际读写飞书文档或制作原生画板时，需要相应工具、Skill 和访问权限。
