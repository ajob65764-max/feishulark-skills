---
name: lark-im
version: 1.0.0
description: "飞书即时消息 IM：发送文本、富文本、卡片、图片、文件，搜索群聊，读取消息，处理卡片交互。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli im --help"
---

# lark-im

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md)。

## 适用场景

- 给用户或群发送消息。
- 搜索群聊、读取 chat_id。
- 发送图片、文件、富文本和交互卡片。
- 回复或处理卡片交互。

## 常用命令

```bash
lark-cli im +messages-send --user-id <open_id> --text "消息内容" --as bot
lark-cli im +messages-send --chat-id <chat_id> --text "消息内容" --as bot
lark-cli im +chat-search --query "群名" --as user
lark-cli im messages get --params '{"message_id":"<message_id>"}' --as user
```

## 注意

发消息前确认接收对象。需要从姓名解析 open_id 时先走 `lark-contact`。
