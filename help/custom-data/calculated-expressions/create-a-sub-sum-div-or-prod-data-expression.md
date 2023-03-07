---
title: 创建SUB、SUM、DIV或PROD数据表达式
description: 了解如何在Adobe的计算字段中使用和创建基本的数学表达式 [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
kt: 8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# 创建SUB、SUM、DIV或PROD数据表达式

在本视频中，您将了解：

* SUB、SUM、DIV和PROD表达式的作用
* 如何在计算字段中创建SUB数据表达式

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12)

## 附加信息：ROUND表达式

### 创建ROUND表达式

ROUND表达式采用任意数字，并将其四舍五入到一定数量的小数位。

大多数情况下，ROUND数据表达式与另一个数据表达式结合使用，当格式字段保留为Text或Number时。

让我们创建一个计算字段，以确定任务中计划小时数和实际登录小时数之间的差异，该差异将需要SUB表达式，如下所示：

**SUB({workRequired}，{actualWorkRequired})**

由于时间以分钟为单位进行跟踪，并且首选格式是以小时为单位显示信息，因此表达式也需要以60除以，如下所示：

**DIV(SUB({workRequired}，{actualWorkRequired})，60)**

如果在自定义表单中构建计算字段时格式更改为数字，则可以在视图中添加字段时更改数字格式。

![具有利用率报告的工作负载均衡器](assets/round01.png)

但是，如果在创建自定义字段时字段格式保留为文本，则无法轻松地在视图中更改格式。 必须使用ROUND表达式以避免在项目中看到类似这样的数字：

![具有利用率报告的工作负载均衡器](assets/round02.png)

<b>在计算字段中使用ROUND数据表达式</b>

ROUND表达式包括表达式的名称(ROUND)，通常包括两个数据点。 这些数据点可以是Workfront中的表达式或字段，后跟一个数字，指示您希望前往的小数位数。

表达式的结构如下所示：ROUND(data point， #)

在计算计划小时数和实际小时数之差的表达式中，使用此表达式 — DIV(SUB({workRequired}，{actualWorkRequired})，60) — 作为第一个数据点。 然后，请确保该表达式中的数字不超过小数点右边的2位。

![具有利用率报告的工作负载均衡器](assets/round03.png)

表达式的编写方式如下所示： ROUND(DIV(SUB({workRequired}，{actualWorkRequired})，60)，2)。
