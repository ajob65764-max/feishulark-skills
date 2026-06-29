# Lark Skills

这是一套面向 Codex / Agent 的飞书（Feishu/Lark）技能包，用于在 AI Agent 工作流中读取、创建、更新和管理飞书相关资源，例如：文档、多维表格、电子表格、云文档空间、日历、消息、邮件、任务、会议纪要、白板等。

> 本仓库只包含技能说明、参考文档、辅助脚本和示例资源；它本身不会包含任何飞书账号权限或密钥。

## 项目内容

仓库中每个 `lark-*` 目录都是一个独立技能，核心入口通常是：

```text
lark-doc/SKILL.md
lark-base/SKILL.md
lark-sheets/SKILL.md
lark-drive/SKILL.md
lark-wiki/SKILL.md
```

当前包含 27 个技能目录，覆盖以下方向：

- 飞书文档：`lark-doc`
- 飞书多维表格：`lark-base`
- 飞书表格：`lark-sheets`
- 飞书云盘：`lark-drive`
- 飞书知识库：`lark-wiki`
- 飞书日历：`lark-calendar`
- 飞书消息 / IM：`lark-im`
- 飞书邮件：`lark-mail`
- 飞书任务：`lark-task`
- 飞书审批：`lark-approval`
- 飞书通讯录：`lark-contact`
- 飞书会议 / 妙记 / 白板：`lark-vc`、`lark-minutes`、`lark-whiteboard`
- 飞书应用与开放平台：`lark-apps`、`lark-openapi-explorer`
- 工作流类技能：`lark-workflow-meeting-summary`、`lark-workflow-standup-report`

## 安装方式

把需要的 `lark-*` 文件夹复制到 Codex / Agent 的 skills 目录中，例如：

```bash
mkdir -p ~/.codex/skills
cp -R lark-doc ~/.codex/skills/
cp -R lark-base ~/.codex/skills/
cp -R lark-sheets ~/.codex/skills/
```

最终结构应该是：

```text
~/.codex/skills/lark-doc/SKILL.md
~/.codex/skills/lark-base/SKILL.md
~/.codex/skills/lark-sheets/SKILL.md
```

复制完成后，重启 Codex / Agent，让系统重新发现技能。

## 使用前提

使用这些技能前，需要先准备好：

1. 可用的 `lark-cli` 或对应飞书开放平台工具。
2. 已完成飞书 / Lark 授权登录。
3. 目标文档、表格、多维表格、知识库、群聊、日历等资源的访问权限。
4. 如果涉及写入操作，需要确认应用权限范围已经开启。

安装技能并不等于自动获得飞书数据权限。最终能否读取或写入，取决于当前登录身份、应用权限、API Scope 和目标资源权限。

## 安全说明

不要把任何账号凭证、Token、私钥或本地登录状态提交到仓库。

## License

暂未选择开源协议。公开发布前，请根据你的使用目的选择并添加合适的 License。
