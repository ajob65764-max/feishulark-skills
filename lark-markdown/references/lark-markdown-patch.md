# lark-markdown patch

对 Markdown 文件进行局部替换。

```bash
lark-cli markdown +patch --file-token <file_token> --pattern "旧文本" --content "新文本" --as user
```

正则替换要注意转义。patch 本质是下载、替换、再覆盖上传。
