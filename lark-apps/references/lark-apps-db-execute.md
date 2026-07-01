# lark-apps db execute

执行妙搭应用数据库 SQL。

## 高风险

涉及删除、更新、清空表、DDL 变更时必须先 dry-run 或让用户确认。不要直接执行不可逆 SQL。
