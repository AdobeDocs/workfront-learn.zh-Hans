---
title: 了解财务访问权限
description: 了解财务访问权限如何让管理员控制谁可以查看和编辑Workfront中跟踪的财务信息。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 5%

---

# 了解财务访问权限

如果贵组织通过以下方式捕获任何财务数据： [!DNL Workfront]，作为系统管理员，您有责任保护和管理有权查看和编辑该信息的用户。

用户查看或编辑财务信息需具备两个条件：

1. 必须在中启用访问权限 [!UICONTROL Access Level].
2. 必须逐个对象授予使用这些访问权限的权限。

例如，可以授予用户查看其访问级别中财务数据的权限，但他们只能查看与其共享的任务中的财务数据，并且在共享该任务中启用了财务查看。

因此，用户可能使用 [!UICONTROL Access Level] 查看财务数据的权限，以便能够查看某些对象上的财务数据，而无法查看其他对象上的财务数据，具体取决于这些对象的各个共享选项。 但是，任何用户都不能查看任何对象上的财务，除非他们有权在他们的帐户中查看财务 [!UICONTROL Access Level].

## [!UICONTROL Access Level] 设置

首先授予对财务数据的整体访问权限 [!DNL Workfront] 许可证类型。

**[!UICONTROL Plan]许可证可以：**

* 管理开票记录
* 管理和查看角色计费和成本率
* 管理和查看用户计费和成本率
* 管理费用
* 查看和编辑财务

**[!UICONTROL Work]许可证可以：**

* 管理费用
* 查看财务

**[!UICONTROL Review]许可证可以：**

* 查看财务

**权限可通过以下方式修改 [!UICONTROL Access Level]. 财务数据访问的三个选项包括：**

* [!UICONTROL No Access]  — 用户将无法查看财务信息。
* [!UICONTROL View]  — 用户可以查看和共享信息。
* [!UICONTROL Edit]  — 用户可以创建、编辑、删除和共享信息。 （仅适用于计划许可证。）

![显示访问级别中常规财务数据选项的图像](assets/setting-up-finances-8.png)

请务必注意， [!UICONTROL View] 和 [!UICONTROL Edit] 选项具有的其他设置 [!UICONTROL Plan] 许可证。 单击 [!UICONTROL View] 按钮来指定这些选项：

**[!UICONTROL View]**

* 查看角色记帐 &amp; 成本率
* 查看用户记帐 &amp; 成本率

![显示访问级别中财务数据视图选项的图像](assets/setting-up-finances-9.png)

**[!UICONTROL Edit]**

这两个选项位于 [!UICONTROL Edit] 选项，以及：

* 编辑角色记帐 &amp; 成本率
* 编辑用户记帐 &amp; 成本率

![显示访问级别中财务数据编辑选项的图像](assets/setting-up-finances-10.png)

>[!NOTE]
>
>有权添加费用的用户还可以查看他们添加的费用及其直接下属添加的费用。
