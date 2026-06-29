# lark-calendar create

创建飞书日程。

## 基本流程

1. 确认标题。
2. 确认开始时间和结束时间。
3. 确认参与人。
4. 确认地点或会议室。
5. 调用 `lark-cli calendar +create`。

## 示例

```bash
lark-cli calendar +create --summary "会议标题" --start "2026-03-26T10:00:00+08:00" --end "2026-03-26T11:00:00+08:00" --as user
```

## 注意

日程属于用户资源，默认使用 `--as user`。创建前需要确认时间和参与人，不能创建完全过去的日程。
