# lark-calendar suggestion

根据时间范围、参会人忙闲和会议时长推荐可用时间块。

## 命令

```bash
lark-cli calendar +suggestion --start "2026-03-26T09:00:00+08:00" --end "2026-03-26T18:00:00+08:00" --duration 60 --as user
```

## 使用场景

- 用户没有给明确时间，只说“找个大家都方便的时间”。
- 用户要会议室但只给了模糊时间范围。
- 需要先推荐时间，再创建日程或查会议室。
