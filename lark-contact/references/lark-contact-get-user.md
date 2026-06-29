# lark-contact get-user

用于已知 `open_id` / `user_id` / `union_id` 时查询用户资料。

## 常用命令

```bash
lark-cli contact +get-user --user-id <open_id> --as bot
lark-cli contact +get-user --user-id <open_id> --user-id-type open_id --as bot
```

## 使用规则

- bot 身份只能查询应用可见范围内的用户。
- user 身份查人通常优先使用 `+search-user`。
- 搜索姓名、邮箱、手机号时不要直接用本命令，先走 `+search-user`。
- 如果只需要给某人发消息，拿到 open_id 后切到 `lark-im`。
