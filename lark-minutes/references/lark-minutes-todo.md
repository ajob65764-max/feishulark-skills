# lark-minutes todo

用于读取或管理妙记里的待办。

## 命令

```bash
lark-cli minutes +todo --minute-token <minute_token> --as user
```

## 路由规则

如果用户说的是：

- 妙记里的待办
- 会议纪要里的待办
- `/minutes/` 链接里的待办
- 妙记 AI 生成的待办

就走本 reference，不要走 `lark-task`。

如果用户说的是普通飞书任务、任务清单、项目待办，则走 `lark-task`。
