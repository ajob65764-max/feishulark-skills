# Upload Status

当前仓库已上传并整理为一套可用的 **核心入口 + 常用 references** 版本。

## 当前定位

这个仓库现在适合：

- 作为 Codex / Agent 的飞书 skill 起步包。
- 快速查找飞书常用能力的操作路径。
- 继续在 GitHub 上补齐、维护、扩展。

需要注意：当前不是原始 386 个文件的逐字完整镜像，而是通过 GitHub 连接器分批上传整理出来的精简常用版。

## 已整理文档

| 文件 | 状态 | 作用 |
|---|---|---|
| `README.md` | 已整理 | 仓库总说明 |
| `SKILLS_INDEX.md` | 已新增 | 技能索引 |
| `INSTALL.md` | 已新增 | 安装说明 |
| `REPOSITORY_STRUCTURE.md` | 已新增 | 目录结构说明 |
| `CONTRIBUTING.md` | 已新增 | 后续维护规则 |
| `.gitignore` | 已新增 | 忽略敏感信息和本地缓存 |

## 已覆盖 skill

- `lark-approval`
- `lark-apps`
- `lark-attendance`
- `lark-base`
- `lark-calendar`
- `lark-contact`
- `lark-doc`
- `lark-drive`
- `lark-event`
- `lark-im`
- `lark-mail`
- `lark-markdown`
- `lark-minutes`
- `lark-note`
- `lark-okr`
- `lark-openapi-explorer`
- `lark-shared`
- `lark-sheets`
- `lark-skill-maker`
- `lark-slides`
- `lark-task`
- `lark-vc`
- `lark-vc-agent`
- `lark-whiteboard`
- `lark-wiki`
- `lark-workflow-meeting-summary`
- `lark-workflow-standup-report`

## 已知限制

### 1. lark-task 入口文件需要手动改名

`lark-task/SKILL.md` 因连接器路径安全拦截，已上传为：

```text
lark-task/skill.md
```

并附带：

```text
lark-task/RENAMING_NOTE.md
```

使用前需要在 GitHub 网页或本地手动改名为：

```text
lark-task/SKILL.md
```

### 2. references 是常用精简版

当前 references 已覆盖常用命令和工作流，但不是原始大包里的全部细节文件。

### 3. 完整包建议用本地 git 补齐

如需把原始 386 个文件完整恢复，建议用 GitHub Desktop 或本地 `git push`，不要继续通过连接器逐文件上传。

## 后续建议

1. 手动把 `lark-task/skill.md` 改成 `lark-task/SKILL.md`。
2. 本地 clone 仓库后，用原始完整包覆盖补齐。
3. 执行一次目录检查，确保每个 `lark-*` 目录都有入口文件。
4. 根据实际使用频率，继续补充缺失 reference。
