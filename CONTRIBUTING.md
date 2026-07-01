# Contributing / 维护规则

这个仓库目前是通过 GitHub 连接器分批上传整理出来的精简常用版。后续如果继续维护，建议按下面规则补齐。

## 新增 skill

每个 skill 必须有：

```text
lark-xxx/SKILL.md
```

`SKILL.md` 应包含：

- skill 名称和用途。
- 什么时候使用。
- 什么时候不要使用。
- 常用命令或 reference 路由。
- 认证、权限和安全提示。

## 新增 reference

reference 放在：

```text
lark-xxx/references/<name>.md
```

命名建议：

```text
lark-doc-fetch.md
lark-base-records-search.md
lark-calendar-schedule-meeting.md
```

保持「skill 名 + 操作名」的格式，方便搜索。

## 高风险操作必须写确认规则

下面这些操作的 reference 里必须明确写“先确认”：

- 删除文件、记录、任务、日程、知识空间。
- 发送邮件、发送消息。
- 批量写入、批量更新、批量移动。
- 开放权限、公开链接、修改可见范围。
- 数据库 SQL 执行。

## 不要提交敏感信息

不要提交：

- 飞书 appSecret
- access token / refresh token
- 私钥
- 本地登录态
- `.env`
- 个人账号凭证
- 客户数据原文

## 补齐原始完整包

如果要把原始 386 个文件完整上传，建议用本地 git 或 GitHub Desktop：

```bash
git clone https://github.com/ajob65764-max/feishulark-skills.git
cp -R /path/to/full-lark-skills/* feishulark-skills/
cd feishulark-skills
git add .
git commit -m "Restore full lark skills package"
git push
```

不要手动逐文件复制大包，容易漏文件，也容易触发路径或内容安全拦截。
