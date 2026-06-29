# lark-event im

IM 事件参考。

## 常见事件

- 消息接收
- 消息反应新增或删除
- 群聊成员变化
- 卡片交互触发

## 使用流程

```bash
lark-cli event list --json
lark-cli event schema im.message.receive_v1 --json
lark-cli event consume im.message.receive_v1 --as bot
```

监听前先用 schema 查看字段结构，再决定 jq 过滤条件。
