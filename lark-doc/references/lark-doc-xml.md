# lark-doc XML

飞书文档 XML 写作格式参考。

## 常用元素

```xml
<title>标题</title>
<h1>一级标题</h1>
<h2>二级标题</h2>
<p>普通段落</p>
<ul><li>列表项</li></ul>
<ol><li>步骤</li></ol>
<blockquote>引用</blockquote>
<callout>提示内容</callout>
```

## 原则

- 文档写入默认使用 XML。
- 标签必须闭合。
- 不要输出不受支持的 HTML 结构。
- 复杂资源块如 sheet、bitable、whiteboard 需要按对应资源块规则处理。
