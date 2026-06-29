---
name: lark-vc-agent
version: 1.0.0
description: "飞书视频会议会中能力：让应用机器人加入或离开正在进行的会议，并读取当前身份可见的会中事件。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli vc --help"
---

# lark-vc-agent

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md) 和 [`../lark-vc/SKILL.md`](../lark-vc/SKILL.md)。

## 适用场景

- 正在开的会议发生了什么。
- 谁加入或离开了会议。
- 当前谁在发言。
- 是否有聊天、共享屏幕等会中事件。
- 需要让机器人加入或离开正在进行的会议。

## 常用流程

```bash
lark-cli vc agent join --meeting-id <meeting_id> --as bot
lark-cli vc agent events --meeting-id <meeting_id> --as bot
lark-cli vc agent leave --meeting-id <meeting_id> --as bot
```

## 边界

- 已结束会议搜索、纪要、逐字稿、录制查询：走 `lark-vc`。
- 未来日程和会议室：走 `lark-calendar`。
