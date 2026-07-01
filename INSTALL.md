# Install

把本仓库里的技能目录复制到 Codex / Agent 的 skills 目录即可。

## 方式一：只安装需要的技能

```bash
mkdir -p ~/.codex/skills
cp -R lark-doc ~/.codex/skills/
cp -R lark-base ~/.codex/skills/
cp -R lark-sheets ~/.codex/skills/
cp -R lark-drive ~/.codex/skills/
```

适合只使用部分飞书能力，例如文档、表格、多维表格。

## 方式二：安装全部 lark 技能

```bash
mkdir -p ~/.codex/skills
cp -R lark-* ~/.codex/skills/
```

复制完成后，重启 Codex / Agent。

## lark-task 特殊处理

当前仓库中：

```text
lark-task/skill.md
```

需要先在 GitHub 网页或本地改名为：

```text
lark-task/SKILL.md
```

否则部分 Agent 可能无法识别该技能入口。

## 使用前检查

确认每个技能目录至少有：

```text
SKILL.md
```

并且当前环境能执行：

```bash
lark-cli --help
```

## 权限提醒

安装 skills 只代表 Agent 知道怎么操作飞书，不代表已经拥有飞书权限。实际读写仍然需要：

- 飞书 / Lark 登录授权
- 目标资源访问权限
- 应用 API scope
- 正确的 user 或 bot 身份
