# lark-event vc

视频会议事件参考。

## 常见场景

- 会议参与者结束会议。
- 会议纪要生成。
- 会议结束后自动触发总结流程。

## 示例

```bash
lark-cli event schema vc.meeting.participant_meeting_ended_v1 --json
lark-cli event consume vc.meeting.participant_meeting_ended_v1 --as user
```

拿到会议 ID 后，可继续走 `lark-vc +detail` 查询会议产物。
