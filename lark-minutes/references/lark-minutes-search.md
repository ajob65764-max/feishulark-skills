# lark-minutes search

搜索用户可见范围内的飞书妙记。

## 命令

```bash
lark-cli minutes +search --query "关键词" --as user
```

## 使用场景

- 用户只知道妙记标题或会议主题。
- 需要先找 `minute_token`。
- 汇总某段时间内的妙记资料。

## 注意

搜索结果多条时，展示标题、时间、创建人和链接，让用户确认目标。拿到 `minute_token` 后再调用 `minutes +detail`。
