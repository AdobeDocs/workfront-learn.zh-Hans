---
title: 了解错误处理指令
description: 了解允许执行继续的错误处理程序指令和阻止执行的错误处理程序指令(位于 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# 了解错误处理指令

在此视频中，您将学习：

* 允许继续执行的三个错误处理程序指令
* 停止执行的两个错误处理程序指令

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12)

## 指令 — 方案继续

### 恢复

* 指定替代输出并提供给遇到错误的模块。
* 后续模块被处理。
* 方案执行状态标记为“成功”。

![恢复指令的图像](assets/troubleshooting-and-error-handling-2.png)

### 中断

* 方案执行的状态存储在未完成执行的队列中，在该队列中可以手动解决错误。 但是，这里提到了一些例外。
* 不会处理后续模块。
* 如果存在未处理的包，则情景会继续正常执行。
* 方案执行状态标记为“警告”。

![Break指令的图像](assets/troubleshooting-and-error-handling-3.png)

### 忽略

* 将忽略该错误，并且不会处理后续模块。
* 如果存在未处理的包，则情景会继续正常执行。
* 方案执行状态标记为“成功”。

![忽略指令的图像](assets/troubleshooting-and-error-handling-4.png)

## 指令 — 方案停止

### 回滚

* 立即停止方案执行，并在所有模块上启动回滚阶段，以尝试将所有模块还原到其初始状态。
* 不会处理后续模块。
* 除少数错误类型外，在方案设置下指定的“连续错误数”后，将停用方案。
* 方案执行状态标记为“error”。

>[!NOTE]
>
>如果未将错误处理程序路由附加到模块，且未选中方案设置下的“允许存储不完整执行”设置，则这是默认行为。

![回滚指令的映像](assets/troubleshooting-and-error-handling-5.png)

### 提交

* 将忽略该错误，并且不会处理后续模块。
* 如果存在未处理的包，则情景会继续正常执行。
* 方案执行状态标记为“成功”。

![提交指令的图像](assets/troubleshooting-and-error-handling-6.png)
