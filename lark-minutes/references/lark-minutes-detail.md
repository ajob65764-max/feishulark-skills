# lark-minutes detail

根据 `minute_token` 获取妙记详情。

## 命令

```bash
lark-cli minutes +detail --minute-token <minute_token> --as user
```

## 常见来源

- 用户给出 `/minutes/` 链接。
- `vc +detail` 返回 `minute_token`。
- 搜索妙记后得到 token。

## 输出处理

如果详情里包含 `note_id`，说明可以继续切到 `lark-note` 查询会议纪要。需要下载音视频或转写内容时，继续使用 `lark-minutes` 相关命令。
