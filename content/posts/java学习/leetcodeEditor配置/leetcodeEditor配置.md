---
title: "leetcodeEditor配置"
date: 2023-07-28T00:37:15+08:00
draft: true
tags: ["java","leetcode"]
categories: ["java学习"]
description: "leetcodeEditor配置"
---
# leetcode editor配置

[//]: # (![img]&#40;leetcodeEditor配置.assets/image-20230515194623200.png&#41;)
<div>
    <img src=leetcodeEditor配置.assets/image-20230515194623200.png width=100% />
</div>
TempFilePath：

```shell
/home/qrpop/IdeaProjects/practice/DataStrucAndAlgo/00-leetCode/src
```

CodeFileName：

```shell
P$!{question.frontendQuestionId}_$!velocityTool.camelCaseName(${question.titleSlug})
```

CodeTemplate：

```shell
package leetcode.editor.cn;

/**
 * ${question.title}
 * @author mqinrui
 * @date $!velocityTool.date()
 */
public class P${question.frontendQuestionId}_$!velocityTool.camelCaseName(${question.titleSlug}){
	 public static void main(String[] args) {
	 	 //测试代码
	 	 Solution solution = new P$!{question.frontendQuestionId}_$!velocityTool.camelCaseName(${question.titleSlug})().new Solution();
	 }
	 
//力扣代码提交区
${question.code}
}

```

TempalteConstant：

```shell
${question.title}	题目标题	示例:两数之和
${question.titleSlug}	题目标记	示例:two-sum
${question.frontendQuestionId}	题目编号
${question.content}	题目描述
${question.code}	题目代码
$!velocityTool.camelCaseName(str)	转换字符为大驼峰样式（开头字母大写）
$!velocityTool.smallCamelCaseName(str)	转换字符为小驼峰样式（开头字母小写）
$!velocityTool.snakeCaseName(str)	转换字符为蛇形样式
$!velocityTool.leftPadZeros(str,n)	在字符串的左边填充0，使字符串的长度至少为n
$!velocityTool.date()	获取当前时间
```


