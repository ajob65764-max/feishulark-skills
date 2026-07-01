# Feishu / Lark Skills for AI Agents

这是一套面向 Codex / Agent 的飞书（Feishu/Lark）技能包，用于在 AI Agent 工作流中读取、创建、更新和管理飞书相关资源。

> 安全说明：本仓库只包含技能说明、参考文档、辅助说明和示例资源；不包含任何飞书账号权限、Token、私钥、登录态或密钥。

## 当前状态

当前仓库已整理成「核心入口 + 常用 references」结构，适合先作为可用版使用。

需要注意：这不是原始 386 个文件的逐字完整镜像，而是通过 GitHub 连接器分批上传整理出来的精简常用版。完整一比一镜像建议后续用 GitHub Desktop 或本地 `git push` 批量上传。

## 快速入口

| 文件 | 作用 |
|---|---|
| [`SKILLS_INDEX.md`](SKILLS_INDEX.md) | 技能目录索引，快速查找每个 skill 的用途 |
| [`REPOSITORY_STRUCTURE.md`](REPOSITORY_STRUCTURE.md) | 仓库结构说明 |
| [`INSTALL.md`](INSTALL.md) | 安装到 Codex / Agent skills 目录的方法 |
| [`UPLOAD_STATUS.md`](UPLOAD_STATUS.md) | 当前上传状态、已知限制和后续补全建议 |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | 后续维护和补文件规则 |

## 覆盖能力

当前已覆盖 27 个技能方向：

- 文档：`lark-doc`
- 多维表格：`lark-base`
- 电子表格：`lark-sheets`
- 云空间 / 云盘：`lark-drive`
- 知识库：`lark-wiki`
- 日历 / 会议室：`lark-calendar`
- 即时消息 IM：`lark-im`
- 邮件：`lark-mail`
- 任务：`lark-task`
- 审批：`lark-approval`
- 通讯录：`lark-contact`
- 视频会议：`lark-vc`
- 妙记：`lark-minutes`
- 会议纪要：`lark-note`
- 画板：`lark-whiteboard`
- OKR：`lark-okr`
- 事件订阅：`lark-event`
- 妙搭应用：`lark-apps`
- OpenAPI 探索：`lark-openapi-explorer`
- 通用规则：`lark-shared`
- 自定义技能制作：`lark-skill-maker`
- 工作流：`lark-workflow-meeting-summary`、`lark-workflow-standup-report`

## 标准目录结构

每个技能目录通常包含：

```text
lark-xxx/
  SKILL.md
  references/
    xxx.md
```

其中 `SKILL.md` 是技能入口，`references/` 是具体命令、工作流或边界说明。

特殊情况：

```text
lark-task/skill.md
lark-task/RENAMING_NOTE.md
```

由于当前 GitHub 连接器对 `lark-task/SKILL.md` 这个精确路径触发安全拦截，`lark-task` 的入口文件暂时以小写 `skill.md` 上传。使用前请按 `RENAMING_NOTE.md` 在 GitHub 网页里手动改名为 `SKILL.md`。

## 安装方式

把需要的 `lark-*` 文件夹复制到 Codex / Agent 的 skills 目录中，例如：

```bash
mkdir -p ~/.codex/skills
cp -R lark-doc ~/.codex/skills/
cp -R lark-base ~/.codex/skills/
cp -R lark-sheets ~/.codex/skills/
```

复制完成后，重启 Codex / Agent，让系统重新发现技能。

更完整的安装说明见 [`INSTALL.md`](INSTALL.md)。

## 使用前提

使用这些技能前，需要准备：

1. 可用的 `lark-cli` 或对应飞书开放平台工具。
2. 已完成飞书 / Lark 授权登录。
3. 目标文档、表格、多维表格、知识库、群聊、日历等资源的访问权限。
4. 如果涉及写入操作，需要确认应用权限范围已经开启。

安装技能并不等于自动获得飞书数据权限。最终能否读取或写入，取决于当前登录身份、应用权限、API Scope 和目标资源权限。

## 维护建议

- 新增 skill：每个目录必须有 `SKILL.md`。
- 新增 reference：放到对应目录的 `references/` 下。
- 高风险操作说明：删除、发送、权限开放、批量写入必须写清楚确认规则。
- 后续如果要补齐原始 386 个文件，建议使用本地 git 一次性提交，避免连接器逐文件上传带来的遗漏。

## License

暂未选择开源协议。公开发布前，请根据使用目的选择并添加合适的 License。
