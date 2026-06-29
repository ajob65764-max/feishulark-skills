---
name: lark-slides
version: 1.0.0
description: "飞书幻灯片：读取、创建和更新飞书 Slides 内容，管理页面、文本、图片和版式。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli slides --help"
---

# lark-slides

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md)。

## 适用场景

- 创建飞书幻灯片。
- 读取或更新已有 slides。
- 添加页面、文本、图片和基本版式。
- 将结构化内容整理成演示文稿。

## 常用命令

```bash
lark-cli slides --help
lark-cli schema slides.<resource>.<method>
lark-cli slides <resource> <method> [flags]
```

## 注意

幻灯片写入前要确认标题、页数、结构和视觉风格。生成本地 PPTX 文件不属于本 skill 范围。
