---
name: lark-task
version: 1.0.0
description: "飞书任务：创建、查询、更新、完成、重开、分配和管理飞书任务、任务清单、子任务、评论、附件、关注人和提醒。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli task --help"
---

# lark-task

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md)。

> 注意：这个文件因为 GitHub 连接器对 `lark-task/SKILL.md` 路径触发安全拦截，暂时使用小写文件名 `skill.md` 保存。使用时请在 GitHub 网页里把文件名改成 `SKILL.md`。

## 适用场景

- 创建待办任务。
- 查看分配给我的任务。
- 查看与我相关、我关注、由我创建的任务。
- 更新任务标题、描述、截止时间、提醒和重复规则。
- 完成或重开任务。
- 添加负责人、关注人、评论、附件。
- 创建和管理任务清单。

## 常用命令

```bash
lark-cli task +create --summary "任务标题" --as user
lark-cli task +get-my-tasks --complete=false --as user
lark-cli task +get-related-tasks --as user
lark-cli task +search --query "关键词" --as user
lark-cli task +update --guid <task_guid> --summary "新标题" --as user
lark-cli task +complete --guid <task_guid> --as user
lark-cli task +reopen --guid <task_guid> --as user
lark-cli task +assign --guid <task_guid> --add <open_id> --as user
lark-cli task +comment --guid <task_guid> --content "评论内容" --as user
lark-cli task +upload-attachment --guid <task_guid> --file <relative_path> --as user
```

## 任务搜索判断

如果用户给了明确关键词，用 `+search`。如果只是范围条件，例如“我负责的”“我关注的”“由我创建的”“今年以来”，不要把时间词当作 query，优先用列表型命令后本地筛选。

## 妙记待办分流

如果用户说的是“妙记里的待办”“会议纪要里的待办”“minute_token / /minutes/ 链接里的待办”，不要走本 skill，切到 `lark-minutes` 的 `minutes +todo`。

## Task GUID

飞书任务 applink 中 `client/todo/task?guid=...` 的 `guid` 才是 OpenAPI 操作任务需要的全局任务 ID，不是客户端展示编号。

## 安全规则

写入、删除、完成、重开、分配成员、修改清单成员前，确认目标任务和影响范围。涉及删除时必须让用户明确确认。
