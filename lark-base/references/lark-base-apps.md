# lark-base apps

多维表格应用 app 相关操作。

## 常用命令

```bash
lark-cli base apps get --params '{"app_token":"<app_token>"}' --as user
```

## 使用场景

- 校验 app_token 是否可访问。
- 获取多维表格基本信息。
- 后续列出 tables、views、fields、records。

## 注意

用户给出 bitable/base 链接时，先提取 app_token，再进入表和记录操作。
