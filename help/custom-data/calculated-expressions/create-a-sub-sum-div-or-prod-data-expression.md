---
title: 创建 SUB、SUM、DIV 或 PROD 数据表达式
description: 了解如何在 Adobe  [!DNL Workfront] 中的计算字段中使用和创建基本数学表达式。
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
jira: KT-8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '386'
ht-degree: 100%

---

# 创建 SUB、SUM、DIV 或 PROD 数据表达式

在本视频中，您将了解到：

* SUB、SUM、DIV 和 PROD 表达式的作用
* 如何在计算字段中创建 SUB 数据表达式

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12&learn=on&enablevpops)

## 附加信息：ROUND 表达式

### 创建 ROUND 表达式

ROUND 表达式接受任何数字并将其四舍五入到一定的小数位数。

大多数情况下，当格式字段保留为文本或数字时，ROUND 数据表达式与另一个数据表达式结合使用。

让我们创建一个计算字段来确定规划的小时数与实际记录任务的小时数之间的差异，这将需要 SUB 表达式，如下所示：

**SUB({workRequired},{actualWorkRequired})**

由于时间以分钟为单位进行跟踪，而首选格式是以小时为单位显示信息，因此表达式还需要除以 60，如下所示：

**DIV(SUB({workRequired},{actualWorkRequired}),60)**

如果在自定义表单中构建计算字段时将格式更改为数字，则可以在视图中添加字段时更改数字格式。

![带有利用率报告的工作负载均衡器](assets/round01.png)

但是，如果创建自定义字段时将字段格式保留为文本，则无法在视图中轻松更改格式。必须使用 ROUND 表达式来避免在项目中看到这样的数字：

![带有利用率报告的工作负载均衡器](assets/round02.png)

<b>在计算字段中使用 ROUND 数据表达式</b>

ROUND 表达式包括表达式的名称 (ROUND)，并且通常包含两个数据点。这些数据点可以是 Workfront 中的表达式或字段，后跟一个数字以指示您想要保留多少位小数。

表达式的结构如下：ROUND(data point, #)

在计算规划小时数与实际小时数之间差异的表达式中，使用此表达式—DIV(SUB({workRequired},{actualWorkRequired}),60)—作为第一个数据点。然后确保该表达式得出的任何数字不超过小数点右侧 2 位。

![带有利用率报告的工作负载均衡器](assets/round03.png)

表达式可以这样写：ROUND(DIV(SUB({workRequired},{actualWorkRequired}),60),2)。
