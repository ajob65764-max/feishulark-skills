# lark-calendar update

更新已有日程。

## 使用前提

必须先定位目标 `event_id`。重复性日程要确认是修改单次实例，还是修改整个系列。

## 常见操作

```bash
lark-cli calendar +update --event-id <event_id> --summary "新标题" --as user
lark-cli calendar +update --event-id <event_id> --start "2026-03-26T14:00:00+08:00" --end "2026-03-26T15:00:00+08:00" --as user
```

## 注意

修改时间、参与人、会议室前，要把变化点复述给用户确认。更新后等待短时间再查询验证。
