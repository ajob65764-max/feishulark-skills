# lark-calendar rsvp

回复日程邀请。

## 命令

```bash
lark-cli calendar +rsvp --event-id <event_id> --status accept --as user
lark-cli calendar +rsvp --event-id <event_id> --status decline --as user
lark-cli calendar +rsvp --event-id <event_id> --status tentative --as user
```

## 状态

- `accept`：接受
- `decline`：拒绝
- `tentative`：暂定

## 注意

回复前确认目标日程，尤其是重复性日程需要确认是单次实例还是整个系列。
