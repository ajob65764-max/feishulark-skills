# lark-base fields

多维表格字段相关操作。

## 常用命令

```bash
lark-cli base fields list --params '{"app_token":"<app_token>","table_id":"<table_id>"}' --as user
```

## 使用规则

写入、更新或搜索记录前，必须先了解字段结构：

- 字段名
- 字段 ID
- 字段类型
- 选项值
- 是否必填

不要凭用户自然语言猜字段类型。
