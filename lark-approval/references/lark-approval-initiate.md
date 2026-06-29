# lark-approval initiate

发起飞书原生审批实例。

## 标准流程

1. `approvals search` 搜索可发起审批定义。
2. `approvals get` 查看审批定义详情、表单字段和流程节点。
3. 构造 `instances create` 请求。
4. 执行前让用户确认审批名称、表单值、审批人和抄送人。
5. 成功后返回 `instance_code` 和审批链接。

## 命令

```bash
lark-cli approval approvals search --data '{"keyword":"请假"}' --as user
lark-cli approval approvals get --params '{"approval_code":"<code>"}' --as user
lark-cli approval instances create --data '{"approval_code":"<code>","form":"[...]"}' --yes --as user
```

## 注意

三方审批定义不要用原生提单接口，返回 `create_link` 让用户通过链接发起。
