---
name: lark-event
version: 1.0.0
description: "飞书/Lark 事件订阅与实时事件消费：用于查看可订阅事件、读取事件结构、监听消息、任务、会议、妙记、画板等事件流。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli event --help"
---

# lark-event

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md)。

## 适用场景

- 查看飞书可订阅事件列表。
- 监听 IM 消息、消息反应、群聊变化。
- 监听任务、会议、妙记、画板等事件。
- 为机器人或自动化工作流建立实时事件处理流程。

## 常用命令

```bash
lark-cli event list --json
lark-cli event schema <EventKey> --json
lark-cli event consume <EventKey> --as bot
lark-cli event status --json
lark-cli event stop --all
```

## 使用原则

1. 先 `event list` 找到合法事件键。
2. 再 `event schema` 查看参数和输出字段。
3. 最后用 `event consume` 监听事件。
4. 监听前确认身份：机器人事件通常用 `--as bot`，用户资源相关事件按实际权限判断。
