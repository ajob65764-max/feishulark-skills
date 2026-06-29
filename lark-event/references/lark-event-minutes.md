# lark-event minutes

妙记事件参考。

## 使用场景

妙记生成后自动触发后续流程，例如：

- 读取妙记详情。
- 生成会议摘要。
- 提取待办。
- 推送到群聊或文档。

## 示例

```bash
lark-cli event schema minutes.minute.generated_v1 --json
lark-cli event consume minutes.minute.generated_v1 --as user
```
