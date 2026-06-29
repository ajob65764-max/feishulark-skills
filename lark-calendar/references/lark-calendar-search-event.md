# lark-calendar search-event

按关键词、时间范围和参与人搜索日程。

## 命令

```bash
lark-cli calendar +search-event --query "关键词" --as user
lark-cli calendar +search-event --query "周会" --start "2026-03-01" --end "2026-03-31" --as user
```

## 使用规则

- 只返回日程摘要信息时，如果需要完整详情，再调用原生日程 get 接口。
- 多条结果时，根据标题、时间、组织者让用户确认目标日程。
- 修改或删除日程前，必须先定位准确的 `event_id`。
