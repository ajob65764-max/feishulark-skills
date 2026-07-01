# lark-drive url token

从飞书 URL 中识别 token。

## 常见类型

- docx 文档：走 `lark-doc`
- sheet 表格：走 `lark-sheets`
- bitable 多维表格：走 `lark-base`
- wiki 节点：走 `lark-wiki`
- 普通文件：走 `lark-drive`

先判断类型，再切换到对应 skill。
