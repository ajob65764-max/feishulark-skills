# lark-calendar agenda

查看指定日期或时间范围内的日程安排。

## 命令

```bash
lark-cli calendar +agenda --as user
lark-cli calendar +agenda --start "2026-03-26T00:00:00+08:00" --end "2026-03-26T23:59:59+08:00" --as user
```

## 规则

- 日程属于用户资源，默认 `--as user`。
- `--start` / `--end` 使用 ISO 8601 或日期格式，不要传自然语言。
- 查询“今天 / 明天 / 本周”时，先把自然语言转换成明确日期。
- 输出时按开始时间排序，已拒绝日程标注出来。
