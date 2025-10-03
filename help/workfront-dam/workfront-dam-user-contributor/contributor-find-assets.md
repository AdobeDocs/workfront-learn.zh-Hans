---
title: 了解作为投稿人如何寻找资源
description: 了解如何在 [!UICONTROL Workfront DAM] 中搜索资源、在文件夹内搜索、简化搜索结果、使用元数据和关键词作为搜索过滤器。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 100%

---

# 了解作为投稿人如何寻找资源

在本视频中，您将学习如何：

* 搜索资源
* 在文件夹内搜索
* 简化搜索结果
* 使用元数据和关键词作为搜索过滤器
* 查看文件夹详细信息
* 查看和更新资源元数据和关键词

>[!VIDEO](https://video.tv.adobe.com/v/3453933/?quality=12&learn=on&enablevpops=1&captions=chi_hans)

## 基本搜索条件

基本搜索会查看文件名、元数据字段、关键词和资源内容（取决于资源类型）。它不包括文件夹名称。

大多数搜索结果都是完全匹配的。“完全匹配”规则的一个例外情况是 [!UICONTROL Workfront DAM] 搜索文件名字段的时候。[!UICONTROL Workfront DAM] 会返回部分匹配文件名的项目，而不仅仅是精确匹配文件名的项目。

## 搜索时的用户运算符

尽管基本搜索功能通常会帮您找到所需的资源，但您可能不时需要使用其他搜索参数。

### 部分匹配

要查找部分匹配项，请在搜索词中添加星号。星号只能用在单词末尾。

### AND 运算符

要查找包含多个搜索词的结果，请在单词之间输入 AND。这些单词可以按任何顺序找到。在所有字段中搜索时，两个单词可能不会出现在同一字段中。例如，Paris AND tower 将会查找在任何字段中同时包含这两个词的资源。

### OR 运算符 

使用 OR 运算符查找包含任何搜索词的资源。例如，Paris OR Arc 将查找包含其中一个单词的资源，但不一定同时包含两个单词。

### 短语

要查找准确的短语，请在单词周围使用双引号。所有单词都将按顺序排列在一起。例如，“Eiffel Tower”会按照这个确切的顺序找到这些单词。

### 负运算符

如果要从搜索结果中排除某个单词，请在该单词前面添加减号 (–)。确保减号和单词之间没有空格。例如，要排除元数据中包含“tower”一词的资源，您的搜索可以设置为 Paris -tower。

### 空字段运算符

要查找在特定元数据字段中没有信息的资源，请按以下格式输入您要搜索的字段：?[xxxxx]。例如，如果您想要查找未分配关键词的资源，请在搜索字段中输入 ?[关键词]。
