# lark-doc media insert

向飞书文档插入本地图片或文件。

```bash
lark-cli docs +media-insert --doc "文档URL或token" --file <relative_path> --as user
lark-cli docs +media-insert --doc "文档URL或token" --from-clipboard --as user
```

路径必须是相对路径。截图或剪贴板图片优先使用 `--from-clipboard`。
