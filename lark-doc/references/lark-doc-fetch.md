# lark-doc fetch

读取飞书文档内容。

## 命令

```bash
lark-cli docs +fetch --doc "文档URL或token" --as user
lark-cli docs +fetch --doc "文档URL或token" --doc-format markdown --as user
lark-cli docs +fetch --doc "文档URL或token" --scope simple --as user
lark-cli docs +fetch --doc "文档URL或token" --scope full --as user
```

## scope 选择

- `simple`：默认读取，适合总结、问答、快速理解。
- `with-ids`：需要块 ID、局部插入、替换、删除时使用。
- `full`：保真编辑、复杂结构分析时使用。

## 注意

读取到嵌入的 sheet、bitable、whiteboard、vc-transcribe-tab 时，需要提取 token 并切到对应 skill。
