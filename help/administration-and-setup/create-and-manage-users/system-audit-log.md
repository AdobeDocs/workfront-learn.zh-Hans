---
title: 了解系统审核日志
description: 了解如何使用系统审核日志来审核更改的时间和项目的时间。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
kt: 10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# 了解系统审核日志

系统审核日志是系统管理员监视当前情况的最佳方法 [!DNL Workfront]. 请将日志视为您的真相来源，了解谁做出了什么更改以及何时做出了更改。

通过转到 [!UICONTROL Preferences] 部分 [!UICONTROL Setup] 的上界。 默认情况下，您会看到过去七天的数据。 更改筛选条件以查看不同日期范围中的数据。

当用户执行某些操作时， [!UICONTROL Workfront] 记录在 [!UICONTROL Audit Logs] 部分 [!UICONTROL Setup] 的上界。

![[!UICONTROL Log Type] 下拉菜单 [!UICONTROL Audit Logs] 页面 [!UICONTROL Setup]](assets/admin-fund-audit-log-1.png)

记录或记录的每个操作都会显示：

* 更改的日期和时间
* 日志类型
* 完成操作的用户的名称
* 对象
* 与操作关联的任何详细信息
* IP地址

![[!UICONTROL Audit Log] 列表](assets/admin-fund-audit-log-2.JPG)

## 导出审核日志

通过导出审核日志数据，系统管理员可以与内部/外部审计员或安全专家共享该信息。 一些组织要求保留某些日志以遵守网络安全条例。 其他用户需要将信息导入安全系统进行分析。

审核日志可以以CSV（以逗号分隔的值）文件导出，该文件可以打开到电子表格应用程序或纯文本编辑器中。 导出一次限制为50,000行，因此，如果总数超过50,000，请使用过滤器缩小列表范围。

![[!UICONTROL Export] 按钮 [!UICONTROL Audit Logs] 页面](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
