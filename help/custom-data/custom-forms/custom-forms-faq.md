---
title: 有关自定义Forms的问题解答
description: 获取有关自定义表单的常见问题解答。
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
kt: 10058
source-git-commit: 7cdce710ecc6fbcdccfe147a40623dc96f07ed2c
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 1%

---

# 有关自定义表单的常见问题

**创建字段后，我是否可以切换其显示类型？ 例如，我可以从下拉菜单更改为复选框吗？**

是. 显示类型可以切换为其他类似的显示类型 — 文本到段落、下拉到复选框或单选按钮等。 有关更改显示类型的更多信息，请参阅创建自定义表单一文。


**能否对多个对象使用相同的自定义表单？ 例如，我为项目任务创建的表单？**

否. 自定义表单与对象具有一对一的关系。 但是，您可以复制自定义表单并将对象更改为所需的表单。


**自定义表单是否可以附加到项目模板？**

是. 这样，从该模板创建的任何项目都将已附加自定义表单。


**我在自定义表单上可以拥有的字段数是否存在限制？**

您最多可以在单个自定义表单上添加500个字段。 但是，如果表单上存在100个以上字段，则性能可能会降低，具体取决于自定义表单的复杂性。 复杂表单的示例包括具有级联参数的表单、计算的自定义数据字段，以及给定字段中的多个值选项。


**我可以附加到项目的自定义表单数量是否存在限制？**

是. 一个对象上最多可附加10个自定义表单。 有关更多信息，请参阅本文将自定义Forms应用到对象。


**我能否停用自定义表单？**

是. 在自定义表单的“表单设置”选项卡中，取消选中“处于活动状态”框。 这会从整个Workfront的任意下拉菜单中删除自定义表单。 但是，如果自定义表单已附加到项目，则表单将保留并保留任何已输入的数据。