# VC domain boundaries

会议相关能力分为几个域：

## 日历 Calendar

用于未来日程、预约会议、会议室、参会人邀请。未来会议先走 `lark-calendar`。

## 视频会议 VC

用于已经发生或正在查询的会议记录。常见入口是 `meeting_id`，可通过 `vc +search` 或日历关联信息获得。

## 会议纪要 Note

用于 AI 智能纪要和逐字稿。入口是 `note_id`，通常从 `vc +detail` 获得。

## 妙记 Minutes

用于录制、音视频、转写、妙记待办等。入口是 `minute_token`。

## 路由总结

- 未来日程：`lark-calendar`
- 历史会议记录：`lark-vc`
- AI 纪要详情：`lark-note`
- 妙记内容和录制：`lark-minutes`
- 正文文档读取：`lark-doc`
