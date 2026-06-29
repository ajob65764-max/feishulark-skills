# lark-im messages reply

回复指定飞书消息。

## 示例

```bash
lark-cli im messages reply --params '{"message_id":"<message_id>"}' --data '{}' --as bot
```

回复前确认原消息、回复内容和身份。机器人回复通常使用 `--as bot`。
