# lark-sheets values get

读取电子表格单元格范围。

## 常用命令

```bash
lark-cli sheets values get --params '{"spreadsheet_token":"<token>","range":"Sheet1!A1:D10"}' --as user
```

## 使用场景

- 读取表格数据。
- 做汇总、分析、检查。
- 更新前先查看现有数据。

## 注意

范围要明确。用户只说“整张表”时，先列出 sheet，再判断合适范围。
