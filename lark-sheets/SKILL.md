---
name: lark-sheets
version: 1.0.0
description: "飞书电子表格：读取、写入、更新单元格和范围，管理 sheet、筛选、格式、图片和批量数据。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli sheets --help"
---

# lark-sheets

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md)。

## 适用场景

- 用户给出 spreadsheet 链接或 token。
- 读取表格数据、写入单元格或范围。
- 新增、复制、删除 sheet。
- 批量整理表格内容。

## 常用命令

```bash
lark-cli sheets spreadsheets get --params '{"spreadsheet_token":"<token>"}' --as user
lark-cli sheets sheets query --params '{"spreadsheet_token":"<token>"}' --as user
lark-cli sheets values get --params '{"spreadsheet_token":"<token>","range":"Sheet1!A1:D10"}' --as user
lark-cli sheets values update --params '{"spreadsheet_token":"<token>","range":"Sheet1!A1"}' --data '{}' --as user
```

## 注意

写入前确认 sheet 名称、范围和数据维度。大批量更新建议先读取现状再提交。
