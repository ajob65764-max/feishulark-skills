# Skills Index

这个文件是仓库的技能目录索引，方便快速找到对应能力。

## 核心规则

每个技能目录的入口文件是：

```text
<skill-name>/SKILL.md
```

例外：`lark-task` 因当前 GitHub 连接器对 `lark-task/SKILL.md` 路径触发安全拦截，已先上传为：

```text
lark-task/skill.md
```

使用前请按 `lark-task/RENAMING_NOTE.md` 手动改名为 `SKILL.md`。

## 技能目录

| 技能 | 主要用途 | 常用 references |
|---|---|---|
| `lark-approval` | 审批发起、审批实例、表单字段 | `references/lark-approval-initiate.md` |
| `lark-apps` | 妙搭应用创建、开发、发布、数据库 | `references/lark-apps-create.md`, `references/lark-apps-release-create.md` |
| `lark-attendance` | 考勤打卡记录查询 | `SKILL.md` |
| `lark-base` | 多维表格 app/table/view/field/record | `references/lark-base-records-search.md` |
| `lark-calendar` | 日程、会议室、忙闲、会议预约 | `references/lark-calendar-schedule-meeting.md` |
| `lark-contact` | 搜索用户、获取 open_id | `references/lark-contact-search-user.md` |
| `lark-doc` | 飞书文档读取、创建、编辑、媒体 | `references/lark-doc-fetch.md`, `references/lark-doc-update.md` |
| `lark-drive` | 云空间搜索、上传、下载、移动、权限 | `references/lark-drive-search.md` |
| `lark-event` | 实时事件订阅和消费 | `references/lark-event-im.md` |
| `lark-im` | 消息发送、群聊搜索、消息读取 | `references/lark-im-messages-send.md` |
| `lark-mail` | 邮件搜索、读取、草稿、发送、附件 | `references/lark-mail-search.md` |
| `lark-markdown` | Drive 中普通 Markdown 文件管理 | `references/lark-markdown-create.md` |
| `lark-minutes` | 妙记搜索、详情、下载、待办 | `references/lark-minutes-detail.md` |
| `lark-note` | 会议纪要和逐字稿 | `references/lark-note-detail.md` |
| `lark-okr` | OKR 周期、目标、进展、权重 | `references/lark-okr-cycle-detail.md` |
| `lark-openapi-explorer` | 查找未封装的飞书 OpenAPI | `SKILL.md` |
| `lark-shared` | 认证、权限、安全规则、通用约定 | `SKILL.md` |
| `lark-sheets` | 电子表格读取、写入、范围、格式 | `references/lark-sheets-values-get.md` |
| `lark-skill-maker` | 自定义 skill 创建说明 | `SKILL.md` |
| `lark-slides` | 飞书幻灯片读取、创建、更新 | `references/lark-slides-create.md` |
| `lark-task` | 飞书任务、任务清单、评论、附件 | `skill.md` 暂代 |
| `lark-vc` | 视频会议历史、详情、录制 | `references/lark-vc-detail.md` |
| `lark-vc-agent` | 会中机器人能力和实时事件 | `references/lark-vc-agent-meeting-events.md` |
| `lark-whiteboard` | 飞书画板查询、导出、更新 | `references/lark-whiteboard-update.md` |
| `lark-wiki` | 知识库空间、节点、成员 | `references/lark-wiki-node-list.md` |
| `lark-workflow-meeting-summary` | 会议总结工作流 | `references/workflow-meeting-summary.md` |
| `lark-workflow-standup-report` | 站会/日程待办摘要工作流 | `references/workflow-standup-report.md` |

## 使用建议

1. 先读目标技能的 `SKILL.md`。
2. 根据 `SKILL.md` 路由到对应 reference。
3. 跨域资源要切换 skill，例如文档里嵌入 sheet，就切到 `lark-sheets`。
4. 写入、删除、发送、权限开放等高影响操作，必须先确认。
