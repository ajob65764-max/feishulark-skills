---
name: lark-base
version: 1.0.0
description: "飞书多维表格 Base：读取和管理 app、table、view、field、record，支持查询、写入、更新、删除记录和字段结构。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli base --help"
---

# lark-base

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md)。

## 适用场景

- 用户给出 bitable / base 链接或 app_token。
- 查询表、视图、字段和记录。
- 新增、更新或删除多维表格记录。
- 调整字段结构或批量处理数据。

## 常用命令

```bash
lark-cli base apps get --params '{"app_token":"<app_token>"}' --as user
lark-cli base tables list --params '{"app_token":"<app_token>"}' --as user
lark-cli base views list --params '{"app_token":"<app_token>","table_id":"<table_id>"}' --as user
lark-cli base fields list --params '{"app_token":"<app_token>","table_id":"<table_id>"}' --as user
lark-cli base records search --params '{"app_token":"<app_token>","table_id":"<table_id>"}' --data '{}' --as user
```

## 注意

写入或删除记录前，必须确认目标表、字段映射和影响范围。字段类型要以实际 schema 为准，不要猜字段结构。
