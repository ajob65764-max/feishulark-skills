# lark-base tables

多维表格 table 相关操作。

## 常用命令

```bash
lark-cli base tables list --params '{"app_token":"<app_token>"}' --as user
lark-cli base tables get --params '{"app_token":"<app_token>","table_id":"<table_id>"}' --as user
```

## 使用规则

- 用户没给 table_id 时，先列出 tables。
- 多个表时展示表名和 table_id，让用户确认。
- 后续字段和记录操作必须使用准确 table_id。
