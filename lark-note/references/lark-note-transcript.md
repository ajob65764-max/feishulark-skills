# lark-note transcript

用于 `unified` 会议纪要获取原始逐字稿或会话记录。

## 命令

```bash
lark-cli note +transcript --note-id <note_id> --as user
```

## 使用条件

- 先用 `note +detail` 获取 `note_display_type`。
- 只有 `note_display_type=unified` 时，逐字稿主要走本命令。
- 普通纪要如果有 `verbatim_doc_token`，优先用 `lark-doc` 读取逐字稿文档。

## 输出处理

输出通常包含说话人、时间戳和文本片段。整理会议纪要时应按时间顺序合并，必要时再总结主题、待办和决策。
