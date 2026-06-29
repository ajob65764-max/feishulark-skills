# lark-vc search

搜索指定时间范围内的视频会议记录。

## 命令

```bash
lark-cli vc +search --start "2026-03-01" --end "2026-03-31" --format json --as user
```

## 使用场景

- 查昨天 / 本周 / 上周开过哪些会。
- 整理一段时间内的会议纪要。
- 找到 meeting_id 后继续查询会议详情。

## 注意

搜索范围不要超过接口限制；长时间范围需要拆分。日历未来会议不走本命令，走 `lark-calendar`。
