# approval instance form control parameters

审批表单 `form` 字段需要按审批定义里的控件类型构造。

## 使用原则

1. 先 `approvals get` 获取表单定义。
2. 不要猜控件 ID、字段类型或 value 结构。
3. 按控件类型分别构造文本、数字、日期、人员、部门、明细等 value。
4. 提交前向用户确认最终表单值。

## 注意

复杂控件、明细表格、附件和人员字段必须严格按 schema 传值。字段缺失或类型不匹配会导致审批创建失败。
