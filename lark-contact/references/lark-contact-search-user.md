# lark-contact search-user

用于按姓名、邮箱、手机号等关键词搜索飞书用户，并获取 `open_id`。

## 常用命令

```bash
lark-cli contact +search-user --query "张三" --as user
lark-cli contact +search-user --query "someone@example.com" --as user
lark-cli contact +search-user --query "张三" --has-chatted --as user
```

## 输出处理

- 如果只命中 1 人，可以继续下一步。
- 如果命中多人，并且后续要发消息、建日程、加权限等有副作用操作，必须把候选列给用户确认。
- 输出时展示姓名、邮箱、部门、open_id，方便用户识别。

## 后续路由

- 发消息：切到 `lark-im`。
- 建日程：切到 `lark-calendar`。
- 加知识库成员：切到 `lark-wiki`。
