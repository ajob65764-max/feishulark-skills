---
name: lark-drive
version: 1.0.0
description: "飞书云空间/云盘：搜索、上传、下载、移动、复制、删除文件，管理权限、评论、版本、导入导出文件。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli drive --help"
---

# lark-drive

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md)。

## 适用场景

- 搜索云空间文件、文档、表格、知识库节点。
- 上传或下载本地文件。
- 移动、复制、删除文件或文件夹。
- 查询文件元信息和链接。
- 管理评论、权限、版本和导入导出。

## 常用命令

```bash
lark-cli drive +search --query "关键词" --as user
lark-cli drive +upload --file <relative_path> --folder-token <folder_token> --as user
lark-cli drive +download --file-token <file_token> --output <relative_path> --as user
lark-cli drive metas batch_query --data '{"request_docs":[]}' --as user
```

## 路由

- 编辑文档正文：走 `lark-doc`。
- 表格数据：走 `lark-sheets`。
- 多维表格数据：走 `lark-base`。
- 知识库结构和成员：走 `lark-wiki`。
