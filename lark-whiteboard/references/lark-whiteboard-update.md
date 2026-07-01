# lark-whiteboard update

更新飞书画板内容。

## 常用命令

```bash
lark-cli whiteboard +update --whiteboard <token> --input-format mermaid --content @diagram.mmd --as user
lark-cli whiteboard +update --whiteboard <token> --input-format plantuml --content @diagram.puml --as user
lark-cli whiteboard +update --whiteboard <token> --input-format svg --content @diagram.svg --as user
lark-cli whiteboard +update --whiteboard <token> --input-format raw --content @nodes.json --as user
```

## 规则

- 用户已提供 Mermaid / PlantUML / SVG 时，按对应格式更新。
- 只微调已有节点时，先 query raw，再改 JSON，再 update raw。
- 更新前确认会覆盖画板当前内容。
