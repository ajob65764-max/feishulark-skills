---
name: lark-minutes
version: 1.0.0
description: "飞书妙记：搜索妙记、查看详情、下载或上传音视频、读取或编辑妙记产物内容、改标题、替换说话人和关键词。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli minutes --help"
---

# lark-minutes

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md)，会议产物相关操作还要阅读 [`../lark-vc/references/vc-domain-boundaries.md`](../lark-vc/references/vc-domain-boundaries.md)。

## 适用场景

- 用户给出 `minute_token` 或妙记链接。
- 搜索妙记、查看妙记标题和关联产物。
- 下载音视频、逐字稿或妙记内容。
- 上传本地音视频生成妙记。
- 修改妙记标题、说话人、关键词或待办。

## 常用命令

```bash
lark-cli minutes +search --query "关键词" --as user
lark-cli minutes +detail --minute-token <minute_token> --as user
lark-cli minutes +download --minute-token <minute_token> --as user
lark-cli minutes +upload --file <relative_path> --as user
lark-cli minutes +title --minute-token <minute_token> --title "新标题" --as user
lark-cli minutes +todo --minute-token <minute_token> --as user
```

## 边界

只按自然语言标题找会议纪要时，先走 `lark-drive` / `lark-vc` 定位；已知妙记 token 时再使用本 skill。
