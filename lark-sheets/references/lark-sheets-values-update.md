# lark-sheets values update

更新电子表格单元格范围。

## 常用命令

```bash
lark-cli sheets values update --params '{"spreadsheet_token":"<token>","range":"Sheet1!A1"}' --data '{}' --as user
```

## 使用规则

- 写入前确认范围和数据维度。
- 多行多列数据要确保数组形状匹配。
- 大批量写入前先展示预览。
