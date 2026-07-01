# lark-sheets sheets

管理电子表格内的工作表 sheet。

## 常用命令

```bash
lark-cli sheets sheets query --params '{"spreadsheet_token":"<token>"}' --as user
```

## 使用规则

- 用户没给 sheet 名称时，先列出 sheets。
- 读写范围时确认 sheet 名称是否正确。
- sheet 名称包含空格或特殊字符时，构造 range 要小心。
