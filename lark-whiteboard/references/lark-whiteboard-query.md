# lark-whiteboard query

查询飞书画板内容，可导出为图片、SVG、代码或原始节点结构。

## 常用命令

```bash
lark-cli whiteboard +query --whiteboard <token> --output-as image --as user
lark-cli whiteboard +query --whiteboard <token> --output-as svg --as user
lark-cli whiteboard +query --whiteboard <token> --output-as code --as user
lark-cli whiteboard +query --whiteboard <token> --output-as raw --as user
```

## 输出选择

- `image`：给用户快速预览。
- `svg`：导出矢量图。
- `code`：查看 Mermaid / PlantUML 等代码来源。
- `raw`：需要精确编辑节点时使用。
