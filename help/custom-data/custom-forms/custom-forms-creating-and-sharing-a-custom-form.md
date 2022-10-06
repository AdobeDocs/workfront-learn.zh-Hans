---
title: 创建和共享自定义表单
description: 了解如何创建自定义表单、向表单中添加唯一字段、使用分区和逻辑组织字段以及与用户共享表单。
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
thumbnail: 335172.png
kt: 8909
exl-id: b37334c7-67d0-4359-9537-dc26843582d1
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 5%

---

# 创建和共享自定义表单

在此视频中，您将学习如何：

* 确定要用于表单的对象
* 以各种格式添加唯一字段
* 使用节和逻辑组织字段
* 与其他用户共享表单

>[!VIDEO](https://video.tv.adobe.com/v/335172/?quality=12)

## 自定义表单可与多种对象类型配合使用

当您单击 [!UICONTROL New Custom Form] 按钮，您可以选择任意数量的对象以在单个自定义表单中使用。 在将自定义表单附加到任何选定对象后，您添加到此表单的所有字段都将可用于这些对象。

![显示 [!UICONTROL New Custom Form] 对象选项](assets/create-custom-form.png)

编辑自定义表单时，您可以看到所有选定的对象类型。 您可以从此列表中添加或删除对象类型。

![自定义表单窗口，显示在表单编辑期间选定的对象类型](assets/edit-custom-form.png)

您可能需要创建一个类型为项目和问题的自定义表单。 附加到问题后，您可以填写与问题相关的任何字段。 之后，如果您决定将问题转换为项目，则自定义表单将自动加载到项目中，并且您放置在问题自定义表单字段中的数据将可用于在项目自定义表单中查看或编辑。

## 自定义字段选项

**[!UICONTROL Label]和 [!UICONTROL Name] 字段**

的 [!UICONTROL Label] 和 [!UICONTROL Name] 自定义字段中的字段的用途各不相同。 [!UICONTROL Label] 是用户将在中看到的字段名称 [!DNL Workfront]. [!UICONTROL Name] 是可与集成一起使用的内容，例如API。

![显示自定义表单窗口 [!UICONTROL Label] 和 [!UICONTROL Name] 字段](assets/custom-forms-field-label-and-name.png)

这样，您就可以灵活地更改面向用户的标签以匹配组织中所做的更改，而不会影响依赖特定字段名称的集成或其他连接。

**[!UICONTROL Text Field with Formatting]**

的 [!UICONTROL Text Field with Formatting ]包含基本文本标记工具，允许用户在自定义表单上填写字段时，在文本上添加粗体、斜体或下划线。

![显示自定义表单窗口 [!UICONTROL Text Field with Formatting] 选项](assets/custom-forms-text-field-with-formatting.png)

该字段还具有15,000个字符的限制，允许有大量空间来提供重要信息，并使用格式设置以便他人阅读。

**[!UICONTROL Typeahead]字段**

的 [!UICONTROL Typeahead] 字段，系统可根据为字段选择的对象自动填充选项列表。

![显示自定义表单窗口 [!UICONTROL Typeahead] 字段选项](assets/custom-forms-typeahead-1.png)

例如，如果您创建 [!UICONTROL Typeahead] 字段“Marketing Manager Approval Name”（营销经理批准名称），然后选择 [!UICONTROL User] 作为引用的对象类型，当用户在自定义表单上填写该字段时，将显示用户名列表。 的 [!UICONTROL Typeahead] 字段用于将自定义数据与系统中捕获的信息连接起来，而无需在下拉字段中手动维护多个选项。

![显示自定义表单窗口 [!UICONTROL Typeahead] 下拉菜单](assets/custom-forms-typeahead-2.png)
