---
{"dg-publish":true,"permalink":"/Md Files/Java概述/","dgPassFrontmatter":true}
---

#### Java应用
- 大数据算法工程师
- Android开发
- 企业级应用
---
#### 如何快速学习

```mermaid
graph LR;
1[①\n需求\n1.工作需要\n2.跳槽对方要求\n3.技术控]-->2[②\n看看能否使用传统技术解决\n1.能解决但不完美\n2.解决不了]-->3[③\n引出我们学习新技术的知识点]
4[④\n学习顺序和步骤\n1.先学习新技术的知识点\n和基本语法,不考虑细节]-->5[⑤\n快速入门,基本程序]-->6[⑥\n开始研究技术的注意事项、使用细节\n使用规范、如何优化]
```

---
#### Java历史
- 什么是程序：==有序指令==的集合
- `.class` 为编译后的文件
- `.java` 为写程序的文件
---
#### Java特点
- 1、面向对象
- 2、健壮性的、强类型语言、异常处理、垃圾自动收集机制
- 3、[[跨平台性.canvas]]`.class`可以在多个平台运行
- 4、[[Md Files/解释型\|解释型]]语言
---
#### Sublime
- Java开发工具
	- IDEA
	- eclipse
	- Sublime (文本编辑器)
---
#### Java运行机制
```mermaid
graph LR;
3[源文件\n.java]--- 1{编译&nbsp;javac} -->字节码文件\n.class ---2{运行&nbsp;java}--> a[JVM for inux] & b[JVM for Windows] & c[JVM for Mac]

```
- Java跨平台性的原因：[[Md Files/JVM\|JVM]] (包含于[[Md Files/JDK\|JDK]]里)
---
#### [[Md Files/JDK\|JDK]] 
- 下载和安装
---
#### 转义字符
- `\t`制表位，实现对齐功能
- `\n`换行符
- `\\`一个\
	- `\`表示转义
- `\"`一个"
- `\'`一个'
- `\r`一个回车 [空降](https://www.bilibili.com/video/BV1fh411y7R8?t=843.3&p=21) 
---
#### Java开发规范
- Java源文件的==基本组成部分==是类(class)
- main方法是固定的，是程序执行入口
- Java语言==区分大小写==
- Java方法由一条条语句组成，分号(`;`)必不可少
- 一个**源文件**中最多有一个public类，可以有其他类，其他类个数不限，但public类只能有一个
	- 编译后，==每一个类都对应一个==`.class`文件
- 如果**源文件**包含一个public类，则文件名==必须按该类名命名== 
	- ==公有类==的类名必须是==文件名称==
- 一个源文件中最多只能有一个public类。其他类个数不限，也可以将==main方法==写在==非public类==中，然后指定运行==非public类==，这样入口方法就是==非public==的main方法。[空降](https://www.bilibili.com/video/BV1fh411y7R8?t=656.3&p=19) 
---
#### 常见错误
- 1、文件名写错
- 2、公共类名与文件名不匹配
- 3、缺少分号、拼写错误、英文中文符号错误
- 4、其他错误
	- 业务逻辑错误
	- 环境错误
- [[Md Files/注释\|注释]] 
---
#### [[Md Files/Java代码规范\|JAVA代码规范]]
---
#### Java API
- [空降](https://www.bilibili.com/video/BV1fh411y7R8?t=250.9&p=46) 
- API：应用程序编程接口
- Java语言提供了大量基础类
---
#### Java类的组织形式
```mermaid
graph TD;
subgraph JDK
	1;2;3;4
end
1[包1] & 2[包2] & 3[包3] & 4[包…]
1-.->a[接口…] & b[类…] & c[异常…] & d[枚举…]
b-.->x[字段] & y["构造器(构造方法)"] & z["成员方法(方法)"]
```
