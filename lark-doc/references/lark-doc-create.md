# lark-doc create

创建飞书在线文档。

## 命令

```bash
lark-cli docs +create --content '<title>标题</title><p>正文</p>' --as user
lark-cli docs +create --doc-format markdown --content '# 标题\n正文' --as user
```

## 格式选择

- 默认 XML，适合复杂样式、callout、grid、checkbox、资源块。
- 用户明确提供 Markdown 文件或说导入 Markdown 时，使用 Markdown。

## 注意

创建前确认标题、正文结构和目标位置。创建成功后返回文档链接。
