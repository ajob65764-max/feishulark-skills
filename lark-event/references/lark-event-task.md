# lark-event task

任务事件参考。

## 适用场景

- 监听任务更新。
- 触发自动化流程。
- 根据任务变更同步到文档、表格或消息。

## 基本流程

```bash
lark-cli event schema task.task.update_user_access_v2 --json
lark-cli event consume task.task.update_user_access_v2 --as user
```

任务事件可能包含任务 ID、变更类型、操作者和更新时间。
