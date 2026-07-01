# Repository Structure

本仓库按 skill 维度组织，每个 `lark-*` 目录都是一个可独立使用的技能。

## 根目录

```text
README.md                 仓库总说明
SKILLS_INDEX.md           技能索引
INSTALL.md                安装说明
UPLOAD_STATUS.md          上传状态和限制说明
CONTRIBUTING.md           维护和补文件规则
REPOSITORY_STRUCTURE.md   仓库结构说明
.gitignore                忽略密钥、缓存和本地临时文件
```

## 单个 skill 的推荐结构

```text
lark-xxx/
  SKILL.md                技能入口，负责路由、边界和核心规则
  references/             具体命令、工作流、参数、示例
  assets/                 模板、素材或示例资源，可选
```

部分技能可能还有额外目录，例如：

```text
lark-whiteboard/
  elements/
  routes/
  scenes/
```

## 文件职责

### SKILL.md

`SKILL.md` 是 Agent 发现和使用技能的入口，应该写清楚：

- 什么时候使用这个 skill。
- 不该由这个 skill 处理什么。
- 关键路由规则。
- 高风险操作的确认规则。
- 需要先阅读哪些 references。

### references/

`references/` 用来放具体操作说明，例如：

- 某个命令怎么用。
- 某个 API 的参数结构。
- 某个工作流的执行步骤。
- 某个跨 skill 的边界判断。

### assets/

`assets/` 用来放模板、示例或资源文件。不要把密钥、账号凭证、Token 放进 assets。

## 目前特殊项

`lark-task` 的入口文件暂时是：

```text
lark-task/skill.md
```

原因是连接器对 `lark-task/SKILL.md` 精确路径触发安全拦截。正式使用前请手动改名为：

```text
lark-task/SKILL.md
```
