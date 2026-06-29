# lark-im messages send

发送飞书消息。

## 示例

```bash
lark-cli im +messages-send --user-id <open_id> --text "消息内容" --as bot
lark-cli im +messages-send --chat-id <chat_id> --text "消息内容" --as bot
```

## 规则

- 给人发消息前先用 `lark-contact` 解析 open_id。
- 给群发消息前先用 `lark-im +chat-search` 查 chat_id。
- 外发消息前确认接收对象和内容。
