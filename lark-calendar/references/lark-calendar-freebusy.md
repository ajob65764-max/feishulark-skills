# lark-calendar freebusy

查询用户主日历忙闲信息。

## 命令

```bash
lark-cli calendar +freebusy --user-ids "ou_xxx,ou_yyy" --start "2026-03-26T09:00:00+08:00" --end "2026-03-26T18:00:00+08:00" --as user
```

## 使用场景

- 约会前查看多人的空闲时间。
- 检查时间冲突。
- 结合 `+suggestion` 推荐会议时间。

## 注意

输出忙闲信息后，需要按本地时区渲染时间。已拒绝日程通常不计入忙碌时段。
