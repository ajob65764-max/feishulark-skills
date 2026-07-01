# lark-drive metas

批量查询云空间资源元信息。

```bash
lark-cli drive metas batch_query --data '{"request_docs":[]}' --as user
```

## 用途

- 查询文档 URL。
- 查询文件类型、标题、所有者。
- 将 token 转换为可展示链接。

一次查询数量受 API 限制，较多资源需要分批。
