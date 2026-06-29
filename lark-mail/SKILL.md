---
name: lark-mail
version: 1.0.0
description: "飞书邮箱：搜索和读取邮件、查看线程、创建草稿、发送邮件、处理附件和邮箱标签。"
metadata:
  requires:
    bins: ["lark-cli"]
  cliHelp: "lark-cli mail --help"
---

# lark-mail

开始前先阅读 [`../lark-shared/SKILL.md`](../lark-shared/SKILL.md)。邮箱通常使用 `--as user`。

## 适用场景

- 搜索邮件、读取邮件详情。
- 查看邮件线程或附件。
- 创建草稿或发送邮件。
- 按条件整理邮件。

## 常用命令

```bash
lark-cli mail messages list --as user
lark-cli mail messages get --params '{"message_id":"<message_id>"}' --as user
lark-cli mail drafts create --data '{}' --as user
lark-cli mail messages send --data '{}' --as user
```

## 安全

发送邮件前必须让用户确认收件人、主题和正文。涉及附件时确认文件路径和权限。
