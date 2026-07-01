# lark-base records search

搜索或读取多维表格记录。

## 常用命令

```bash
lark-cli base records search --params '{"app_token":"<app_token>","table_id":"<table_id>"}' --data '{}' --as user
```

## 使用场景

- 读取表内数据。
- 按条件筛选记录。
- 根据字段查找匹配行。
- 做数据汇总、统计和核对。

## 注意

分页结果需要继续翻页。输出时尽量用字段名而不是字段 ID。
