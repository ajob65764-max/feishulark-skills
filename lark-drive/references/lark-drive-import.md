# lark-drive import

导入本地文件为飞书在线文档或其他云空间资源。

```bash
lark-cli drive +import --file <relative_path> --type docx --as user
```

## 注意

导入 Markdown 为在线文档时，通常走 Drive import；创建原生 `.md` 文件时走 `lark-markdown`。
