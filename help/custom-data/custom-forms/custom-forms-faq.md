---
title: 有关自定义表单的问题解答
description: 获取有关自定义表单的常见问题的解答。
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
jira: KT-10058
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 88%
---
# 有关自定义表单的常见问题

**创建字段后可以切换字段的显示类型吗？ 例如，我可以从下拉菜单更改为复选框吗？**

可以。 该显示类型可以切换为另一种类似的显示类型 — 文本到段落、下拉列表到复选框或单选按钮等。有关更改显示类型的更多信息，请参阅创建自定义表单一文。


**我可以对多个对象使用相同的自定义表单吗？ 例如，我为项目任务创建的表单？**

不可以。 自定义表单与对象具有一对一的关系。 但是，您可以复制自定义表单并将对象更改为所需的对象。


**自定义表单可以附加到项目模板中吗？**

可以。 这样，从该模板创建的任何项目都会已经附有自定义表单。


**自定义表单上可以包含的字段数量是否有限制？**

您最多可以在单个自定义表单上添加 500 个字段。 但是，当表单上存在超过 100 个字段时，性能可能会下降，具体取决于自定义表单的复杂性。 复杂表单的示例包括具有级联参数的表单、带有计算自定义数据字段的表单以及给定字段中具有多值选项的表单。


**我可以附加到项目中的自定义表单的数量是否有限制？**

是的。 您最多可以在一个对象上附加 10 个自定义表单。 有关更多信息，请参阅本文——《将自定义表单应用于对象》。


**我可以停用自定义表单吗？**

可以。 在自定义表单的“表单设置”选项卡中，取消选中“处于活动状态”框。 这将会从整个 Workfront 的任何下拉菜单中删除自定义表单。 但是，如果自定义表单已附加到项目，则该表单会保留，并会保留已输入的所有数据。