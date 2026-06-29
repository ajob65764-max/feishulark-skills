# lark-event whiteboard

画板事件参考。

## 使用场景

- 监听指定画板更新。
- 画板更新后导出预览图。
- 触发文档或消息同步。

## 示例

```bash
lark-cli event schema board.whiteboard.updated_v1 --json
lark-cli event consume board.whiteboard.updated_v1 -p whiteboard_id=<token> --as user
```
