# lark-mail search

搜索飞书邮箱邮件。

## 常用命令

```bash
lark-cli mail messages list --as user
lark-cli mail messages list --params '{"query":"关键词"}' --as user
```

## 使用场景

- 按关键词搜索邮件。
- 查找某个发件人、主题或附件。
- 为后续读取详情、创建草稿或回复邮件定位 message_id。

## 注意

邮箱通常属于用户资源，默认 `--as user`。搜索结果多条时，展示发件人、主题、时间和摘要。
