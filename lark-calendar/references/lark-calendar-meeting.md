# lark-calendar meeting

通过日程事件 ID 获取关联的视频会议信息。

## 命令

```bash
lark-cli calendar +meeting --event-ids <event_id> --as user
```

## 输出

可能包含：

- `meeting_id`
- `meeting_note`
- 会议链接
- 与日程绑定的会议产物信息

## 路由

拿到 `meeting_id` 后，如需进一步查询会议纪要、妙记、录制和参会人，切到 `lark-vc`。
