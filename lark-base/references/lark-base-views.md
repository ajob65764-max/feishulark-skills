# lark-base views

多维表格视图相关操作。

## 常用命令

```bash
lark-cli base views list --params '{"app_token":"<app_token>","table_id":"<table_id>"}' --as user
```

## 使用场景

- 按视图读取记录。
- 查找用户口头提到的“表格视图”。
- 确定筛选、排序、隐藏字段等视图上下文。

## 注意

视图不是表。写入记录时仍然需要 table_id 和字段结构。
