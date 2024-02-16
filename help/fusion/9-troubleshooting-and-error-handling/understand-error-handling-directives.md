---
title: 了解错误处理指令
description: 了解  [!DNL Adobe Workfront Fusion] 中允许继续执行以及停止执行的错误处理程序指令。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
recommendations: noDisplay,noCatalog
doc-type: video
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '318'
ht-degree: 100%

---

# 了解错误处理指令

在本视频中，您将了解到：

* 允许继续执行的三个错误处理程序指令
* 停止执行的两个错误处理程序指令

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on)

## 指令——场景继续

### 恢复

* 指定替代输出并将其提供给遇到错误的模块。
* 处理后续模块。
* 场景执行状态标记为“成功”。

![“恢复”指令的图像](assets/troubleshooting-and-error-handling-2.png)

### 间断

* 场景执行的状态存储在未完成执行的队列中，在该队列中可以手动解决错误。然而，这里提到了一些例外情况。
* 未处理后续模块。
* 如果存在未处理的捆绑包，则场景执行会正常继续进行。
* 场景执行状态标记为“警告”。

![简单指令的图像](assets/troubleshooting-and-error-handling-3.png)

### 忽略

* 该错误会被忽略，并且后续模块不会受到处理。
* 如果存在未处理的捆绑包，则场景执行会正常继续进行。
* 场景执行状态标记为“成功”。

![忽略指令的图像](assets/troubleshooting-and-error-handling-4.png)

## 指令——场景停止

### 回滚

* 场景执行立即停止，并在所有模块上启动回滚阶段，试图将它们全部恢复到初始状态。
* 未处理后续模块。
* 除少数错误类型外，在达到“场景”设置下指定的“连续错误数”之后，该场景将会被停用。
* 场景执行状态标记为“错误”。

>[!NOTE]
>
>如果没有将错误处理程序路由附加到该模块，并且未选中“场景”设置下的“允许存储未完成的执行”设置，则这是默认的行为。

![回滚指令的图像](assets/troubleshooting-and-error-handling-5.png)

### 提交

* 该错误会被忽略，并且后续模块不会受到处理。
* 如果存在未处理的捆绑包，则场景执行会正常继续进行。
* 场景执行状态标记为“成功”。

![承诺指令的图像](assets/troubleshooting-and-error-handling-6.png)
