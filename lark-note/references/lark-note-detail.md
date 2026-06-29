# lark-note detail

用于已知 `note_id` 时获取会议纪要详情、展示类型和相关文档 token。

## 命令

```bash
lark-cli note +detail --note-id <note_id> --as user
```

## 关键字段

- `note_display_type`：`normal` / `unified` / `unknown`
- `note_doc_token`：AI 智能纪要文档 token
- `verbatim_doc_token`：普通纪要的逐字稿文档 token
- `shared_doc_tokens`：会中共享文档

## 路由

- 读取纪要正文：拿 `note_doc_token` 后切到 `lark-doc`。
- `normal` 逐字稿：用 `verbatim_doc_token` 走 `lark-doc`。
- `unified` 逐字稿：走 `note +transcript`。
