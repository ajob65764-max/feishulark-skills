# lark-vc detail

根据 `meeting_id` 获取会议详情和会议产物信息。

## 命令

```bash
lark-cli vc +detail --meeting-ids <meeting_id> --as user
lark-cli vc +detail --meeting-ids "id1,id2,id3" --as user
```

## 关键字段

- `note_id`：会议纪要 ID，后续走 `lark-note`。
- `minute_token`：妙记 token，后续走 `lark-minutes`。
- `recording`：录制信息。
- 参会人和时间信息。

## 路由

- 拿到 `note_id` → `lark-note`。
- 拿到 `minute_token` → `lark-minutes`。
- 需要正文 → 再走 `lark-doc`。
