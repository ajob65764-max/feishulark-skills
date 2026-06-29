# lark wiki token routing

当用户给出 wiki 链接或 token 时，要先判断它是知识库节点、文档 token 还是 Drive 文件。

## 规则

- `/wiki/` 链接优先走 `lark-wiki`。
- 如果要编辑正文，先解析出文档 token，再走 `lark-doc`。
- 如果要移动、复制、成员管理，留在 `lark-wiki`。
- 不要因为域名不是标准飞书域名就退回 WebFetch。
