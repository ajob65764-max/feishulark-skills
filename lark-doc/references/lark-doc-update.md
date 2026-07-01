# lark-doc update

更新飞书文档内容。

## 常见命令

```bash
lark-cli docs +update --doc "文档URL或token" --command append --content '<p>新增内容</p>' --as user
lark-cli docs +update --doc "文档URL或token" --command str_replace --old-text "旧文本" --new-text "新文本" --as user
lark-cli docs +update --doc "文档URL或token" --command overwrite --content '<title>新标题</title><p>正文</p>' --as user
```

## 使用规则

- 已知旧文本改新文本，优先 `str_replace`。
- 需要精确插入、替换、删除块时，先 `+fetch --scope with-ids`。
- `overwrite`、`block_replace`、`block_delete` 后不要复用旧 block_id。

## 安全

覆盖、删除、批量替换前必须确认影响范围。
