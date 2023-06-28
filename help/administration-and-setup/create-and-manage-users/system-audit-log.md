---
title: 了解系统审核日志
description: 了解如何使用系统审核日志来查看何时对项目进行了更改以及何时对项目进行了更改。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# 了解系统审核日志

系统审核日志是系统管理员监视当前状况的最佳方法 [!DNL Workfront]. 将日志视为由谁更改了哪些内容以及何时更改了哪些内容的真实来源。

访问审核日志，方法是转到 [!UICONTROL Preferences] 中的部分 [!UICONTROL Setup] 区域。 默认情况下，您会看到过去七天的数据。 更改筛选条件以查看不同日期范围的数据。

当用户执行某些操作时， [!UICONTROL Workfront] 将它们记录在 [!UICONTROL Audit Logs] 部分 [!UICONTROL Setup] 区域。

![[!UICONTROL Log Type] 上的下拉菜单 [!UICONTROL Audit Logs] 页面位置 [!UICONTROL Setup]](assets/admin-fund-audit-log-1.png)

记录或记录的每个操作都会显示：

* 更改日期和时间
* 日志类型
* 完成操作的用户的名称
* 对象
* 与操作关联的任何详细信息
* IP地址

![[!UICONTROL Audit Log] 列表](assets/admin-fund-audit-log-2.JPG)

## 导出审核日志

导出审核日志数据可让系统管理员与内部/外部审核员或安全专家共享信息。 有些组织要求保留某些日志，以遵守网络安全法规。 其他客户需要导入安全系统的信息进行分析。

审核日志可导出为CSV（逗号分隔值）文件，该文件可在电子表格应用程序或纯文本编辑器中打开。 导出限制为一次最多50,000行，因此如果总数超过50,000，请使用过滤器缩小列表范围。

![[!UICONTROL Export] 按钮打开 [!UICONTROL Audit Logs] 页面](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
