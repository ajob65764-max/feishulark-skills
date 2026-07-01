# lark-sheets url token

从飞书电子表格链接中提取 spreadsheet_token、sheet_id 和 range。

## 规则

- 链接指向电子表格时，使用 `lark-sheets`。
- 如果文档中嵌入 `<sheet token="...">`，提取 token 后切到本 skill。
- 如果是多维表格 bitable/base 链接，切到 `lark-base`。
