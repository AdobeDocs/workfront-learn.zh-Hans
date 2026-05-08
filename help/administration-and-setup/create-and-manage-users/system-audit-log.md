---
title: 了解系统审核日志
description: 了解如何使用系统审阅日志来查看何时进行了更改以及何时对项目进行更改。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
TQID: https://experienceleague.adobe.com/xMxWQ53TUXVjS-H8EuK3nf7jt8v4vUgKoZVsmApc-JM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 251
ht-degree: 100%

---

# 了解系统审核日志

系统审核日志是系统管理员关注 [!DNL Workfront] 运行情况的最佳方式。 将日志视为谁在何时进行了哪些更改的事实来源。

通过前往 [!UICONTROL Setup] 区域的 [!UICONTROL Preferences] 部分访问审核日志。 默认情况下，您会看到过去 7 天的数据。 更改过滤条件以查看不同日期范围的数据。

当用户执行某些操作时，[!UICONTROL Workfront] 会在 [!UICONTROL Setup] 区域的 [!UICONTROL Audit Logs] 部分中记录它们。

![[!UICONTROL Log Type] 下拉菜单，在 [!UICONTROL Audit Logs] 页面上，位于 [!UICONTROL Setup]](assets/admin-fund-audit-log-1.png)

记录的每个操作都会显示：

* 更改的日期和时间
* 日志类型
* 完成该操作的用户的名称。
* 对象
* 与操作相关的任何详细信息
* IP 地址

![[!UICONTROL Audit Log]列表](assets/admin-fund-audit-log-2.JPG)

## 导出审核日志

导出审核日志数据允许系统管理员与内部/外部审核员或安全专家共享信息。 一些组织要求保留某些日志以遵守网络安全法规。 其他组织需要将信息导入安全系统进行分析。

审核日志可以导出为 CSV（逗号分隔值）文件，该文件可以在电子表格应用程序或纯文本编辑器中打开。 一次导出的行数限制为 50,000 行，因此如果总数超过 50,000 行，请使用过滤器缩小列表范围。

![[!UICONTROL Export] 按钮，在 [!UICONTROL Audit Logs] 页面上](assets/admin-fund-audit-log-3.png)

<!--
learn more URLs
Audit logs
Managing audit logs
-->
