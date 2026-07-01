# lark-mail read

读取邮件详情。

## 常用命令

```bash
lark-cli mail messages get --params '{"message_id":"<message_id>"}' --as user
```

## 输出处理

展示主题、发件人、收件人、时间、正文摘要和附件列表。需要线程上下文时继续读取 thread。
