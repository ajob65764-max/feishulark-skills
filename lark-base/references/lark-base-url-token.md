# lark-base url token

从多维表格 URL 中提取 app_token、table_id 和 view_id。

## 规则

- `base` 或 `bitable` 链接通常包含 app_token。
- URL 里可能包含 table_id 或 view_id。
- 如果没有 table_id，先调用 tables list。
- 如果没有 view_id，但用户提到视图，先调用 views list。
