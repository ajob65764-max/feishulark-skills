# lark-doc resource cover

下载、更新或删除 Docx 封面图。

```bash
lark-cli docs +resource-download --doc "文档URL或token" --type cover --as user
lark-cli docs +resource-update --doc "文档URL或token" --type cover --file <relative_path> --as user
lark-cli docs +resource-delete --doc "文档URL或token" --type cover --as user
```

`resource-*` 目前主要用于封面资源，普通图片和附件走 media 命令。
