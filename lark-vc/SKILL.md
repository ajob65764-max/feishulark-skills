---
name: lark-vc
version: 1.0.0
description: "飞书视频会议：搜索历史会议记录、查询会议产物、查看参会人快照。查询未来日程走 lark-calendar，会中实时能力走 lark-vc-agent。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli vc --help"
---

# lark-vc

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md) 和 [`references/vc-domain-boundaries.md`](references/vc-domain-boundaries.md)。

## 适用场景

- 查已经结束的视频会议。
- 根据会议 ID 获取纪要、妙记、参会人等信息。
- 查询某段时间内的历史会议。
- 从会议记录继续定位 note_id 或 minute_token。

## 常用命令

```bash
lark-cli vc +search --start <date> --end <date> --as user
lark-cli vc +detail --meeting-ids <meeting_id> --as user
lark-cli vc +participants --meeting-id <meeting_id> --as user
```

## 路由规则

- 未来日程、预约会议、会议室：走 `lark-calendar`。
- 已结束会议和会议产物：走本 skill。
- 会中实时加入、离开、发言、聊天事件：走 `lark-vc-agent`。
- 纪要正文读取：拿到 token 后走 `lark-note` 或 `lark-doc`。
