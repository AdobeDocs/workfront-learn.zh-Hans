---
title: 在中查找和组织资源 [!UICONTROL Workfront DAM]
description: 了解如何搜索资产、在文件夹中搜索、简化搜索结果、将元数据和关键字用作搜索筛选器等，请参阅 [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 参与者：查找资源

在本视频中，您将了解如何：

* 搜索资源
* 在文件夹中搜索
* 简化搜索结果
* 使用元数据和关键字作为搜索过滤器
* 查看文件夹详细信息
* 查看和更新资源元数据和关键字

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on)

## 基本搜索条件

基本搜索会查看文件名、元数据字段、关键字和资源内容（具体取决于资源类型）。 它不包括文件夹名称。

大多数搜索结果都是完全匹配的。 此“完全匹配”规则的例外情况是 [!UICONTROL Workfront DAM] 搜索文件名字段。 [!UICONTROL Workfront DAM] 返回部分文件名匹配项，而不仅仅是精确的文件名匹配项。

## 搜索时的用户运算符

尽管基本搜索功能通常会找到您需要的资源，但您有时可能需要使用其他搜索参数。

### 部分匹配

要查找部分匹配项，请在搜索词中添加星号。 星号只能用于单词的结尾。

### AND运算符

要查找包含多个搜索词的结果，请在搜索词之间输入AND。 这些字可以按任意顺序找到。 跨所有字段搜索时，两个单词可能不在同一字段中。 例如，Paris AND Tower将查找在任何字段中同时包含这两个词的资产。

### OR运算符

使用OR运算符查找包含任何搜索词的资源。 例如，Paris OR Arc将查找包含以下任一词的资产，但不一定同时包含这两个词的资产。

### 短语

要找到确切的短语，请在单词前后使用双引号。 所有单词将按顺序一起找到。 例如，“埃菲尔铁塔”会按照该顺序找到这些单词。

### 负运算符

如果要从搜索结果中排除某个单词，请在该单词前放置一个减号(-)。 确保减号与单词之间没有空格。 例如，要排除元数据中包含“tower”一词的资产，可将搜索设置为Paris -tower。

### 空字段运算符

要查找在特定元数据字段中没有任何信息的资源，请使用此格式输入要搜索的字段：？[xxxxx]. 例如，如果要查找未分配关键字的资源，请输入？[关键词] 在搜索字段中。
