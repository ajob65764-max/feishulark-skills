# lark-doc Markdown

当用户明确要求 Markdown、导入 Markdown 文件或已有内容是 Markdown 时使用。

## 示例

```bash
lark-cli docs +create --doc-format markdown --content '# 标题\n\n正文' --as user
lark-cli docs +update --doc "文档URL或token" --command append --doc-format markdown --content '## 新增章节' --as user
```

## 注意

Markdown 适合普通标题、段落、列表、表格。复杂飞书样式建议使用 XML。
