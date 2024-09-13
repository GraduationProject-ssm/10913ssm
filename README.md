# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# 10913ssm毕业设计管理系统设计

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1Sh44eDEx6?p=14)


# 系统概述
进过系统的分析后，就开始记性系统的设计，系统设计包含总体设计和详细设计。总体设计只是一个大体的设计，经过了总体设计，我们能够划分出系统的一些东西，例如文件、文档、数据等。而且我们通过总体设计，大致可以划分出了程序的模块，以及功能。但是只是一个初步的分类，并没有真正的实现。

整体设计，只是一个初步设计，而且，对于一个项目，我们可以进行多个整体设计，通过对比，包括性能的对比、成本的对比、效益的对比，来最终确定一个最优的设计方案，选择优秀的整体设计可以降低开发成本，增加公司效益，从这一点来讲，整体设计还是非常重要的。

` `毕业设计管理系统 工作原理图如图4-1所示：

![](/md/blog.013.png)

图4-1 系统工作原理图
## 4.2 系统结构设计
系统架构图属于系统设计阶段，系统架构图只是这个阶段一个产物，系统的总体架构决定了整个系统的模式，是系统的基础。 毕业设计管理系统 的整体结构设计如图4-2所示。

![](/md/blog.014.png)

图4-2 系统结构图
## 4.3数据库设计
数据库是计算机信息系统的基础。目前，电脑系统的关键与核心部分就是数据库。数据库开发的优劣对整个系统的质量和速度有着直接影响。
### 4.3.1 数据库设计原则
数据库的概念结构设计采用实体—联系（E-R）模型设计方法。E-R模型法的组成元素有：实体、属性、联系，E-R模型用E-R图表示，是提示教师工作环境中所涉及的事物，属性则是对实体特性的描述。在系统设计当中数据库起着决定性的因素。下面设计出这几个关键实体的实体—关系图。
### 4.3.2 数据库实体
数据模型中的实体（Entity），也称为实例，对应现实世界中可区别于其他对象的“事件”或“事物”。例如，公司中的每个教师，家里中的每个家具。

本系统的E-R图如下图所示：

1、教师实体图如图4-3所示：

![](/md/blog.015.png)

图4-3教师实体图

2、学生信息实体图如图4-4所示：

![](/md/blog.016.png)

图4-4学生信息实体图

3、管理员信息管理实体图如图4-5所示：

![](/md/blog.017.png)

图4-5管理员信息管理实体图

4、在线选题管理实体图如图4-6所示：


![](/md/blog.018.png)

图4-6在线选题管理实体图


### 4.3.3 数据库表设计
数据库的表信息属于设计的一部分，下面介绍数据库中的各个表的详细信息。

表 guanliyuanxinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|PRIMARY KEY|
|username|varchar|50|DEFAULT NULL|
|pwd|varchar|50|DEFAULT NULL|
|cx|varchar|50|DEFAULT NULL|

表3 xuesheng表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|10|PRIMARY KEY|
|xueshengxuehao|int|50|DEFAULT NULL|
|xueshengxingming|varchar|50|DEFAULT NULL|
|xingbie|varchar|50|DEFAULT NULL|
|nianji|varchar|50|DEFAULT NULL|
|banji|varchar|50|DEFAULT NULL|
|shenfenzheng|varchar|50|DEFAULT NULL|
|lianxidianhua|varchar|50|DEFAULT NULL|
表5 jiaoshi数据表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|PRIMARY KEY|
|jiaoshigonghao|varchar|50|DEFAULT NULL|
|jiaoshixingming|varchar|50|DEFAULT NULL|
|mima|varchar|50|DEFAULT NULL|
|zhicheng|varchar|50|DEFAULT NULL|
|lianxidianhua|int|10|DEFAULT NULL|
|shenfenzheng|int|500|DEFAULT NULL|
表6`zaixianxuanti数据表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|PRIMARY KEY|
|ketitimu|varchar|10|DEFAULT NULL|
|tupian|varchar|500|DEFAULT NULL|
|jianjie|varchar|20|DEFAULT NULL|
|jiaoshigonghao|varchar|4|DEFAULT NULL|
|fabushijian|varchar|20|DEFAULT NULL|
|sfsh|varchar|20|DEFAULT NULL|
|shhf|varchar|20|DEFAULT NULL|
表6`xueshengtiwen数据表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|PRIMARY KEY|
|woyaotiwen|varchar|10|DEFAULT NULL|
|xueshengxuehao|varchar|500|DEFAULT NULL|
|xueshengxingming|varchar|20|DEFAULT NULL|
|jiaoshigonghao|varchar|4|DEFAULT NULL|
|jiaoshixingming|varchar|20|DEFAULT NULL|
|tiwenshijian|varchar|20|DEFAULT NULL|
`   `表6`laoshidayi数据表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|PRIMARY KEY|
|laoshidayi|varchar|10|DEFAULT NULL|
|xueshengxuehao|varchar|500|DEFAULT NULL|
|xueshengxingming|varchar|20|DEFAULT NULL|
|jiaoshigonghao|varchar|4|DEFAULT NULL|
|jiaoshixingming|varchar|20|DEFAULT NULL|
|dayishijian|varchar|20|DEFAULT NULL|
#   
# 5系统界面实现
## 5.1 前台功能模块
网站首页
## 网页首页电影订票系统模块如下：首页、在线选题、论坛、个人中心后台管理等功能图5-1
![](/md/blog.019.png)

`                   `![](/md/blog.020.png)

网页前台页面效果图如图5-1所示：

网页前台在线选题效果图如图5-2所示

![](/md/blog.021.png)

网页前台在线选题效果图如图5-2所示

学生在注册完个人信息后会跳转到登录界面上，输入注册的登录账号及密码后才可登录。网页前台学生注册页面如图5-3所示

![](/md/blog.022.png)

`                              `![](/md/blog.023.png)

前台学生注册登录页面如图5-3所示
## 5.2  管理员功能模块
管理员输入个人的账号、密码登录系统，这时候系统的数据库就会在进行查找相关的信息，如果我们输入的账号、密码不正确，数据库就会提示出错误的信息提示，同时会提示管理员重新输入输入自己的账号、密码和验证码，直到账号密码输入成功后，会提登录成功的信息。网站管理员登录效果图如图5-4所示：

![](/md/blog.024.png)     
图5-4登录界面
### 5.2.1 学生信息
管理员对学生信息进行学可以进行编辑生学号、学生姓名 、密码 、性别、 年级、 班级 、身份证、 联系电话添加、删除、修改以及查看、修改密码等操作。程序成效图如下图5-5所示:

![](/md/blog.025.png)

图5-5学生信息界面图
### 5.2.2 教师管理
管理员对教师获取教师工号 教师姓名 密码 职称 联系电话 身份证  进行添加、删除、修改以及查看等操作。程序效果图如下图5-6所示：

![](/md/blog.026.png)

图5-6教师管理界面
### 5.2.3 系统管理
` `管理员通过系统管理页面查看轮播图、新闻资讯等进行上传图片进行添加、删除、修改以及查看并对整个系统进行维护等操作。程序效果图如下图5-7所示：

![](/md/blog.027.png)

图5-7系统管理 界面

### 5.2.4 在线选题管理 
管理员对在线选题获取课题题目 图片 教师工号 发布时间 审核回复 审核等信息进行添加、查看、修改以及删除等操作。程序效果图如下图5-8所示：

![](/md/blog.028.png)

图5-8在线选题界面
### 5.2.5系统管理
管理员对系统管理进行删除、修改以及查看等操作。程序效果图如下图5-9所示：

![](/md/blog.029.png)

图5-9系统管理界面
### 5.2.6在线选题管理
管理员对在线选题管理信息进行编辑课题题目、图片 、教师工号 、发布时间 、审核回复、 审核修改、审核、删除以及查看等操作。程序效果图如下图5-10所示：

![](/md/blog.030.png)

图5-10在线选题管理界面



### 5.2.7中期报告管理
管理员对中期报告管理信息进行修改、审核、删除以及查看等操作。程序效果图如下图5-11所示：

![](/md/blog.031.png)

图5-11中期报告管理界面


### 5.2.8毕业论文管理
管理员对毕业论文管理信息进行修改、审核、删除以及查看等操作。程序效果图如下图5-12所示：

![](/md/blog.032.png)

图5-12毕业论文管理界面

### 5.2.9学生提题管理
管理员对学生提题信息进行修改、审核、删除以及查看等操作。程序效果图如下图5-13所示：

![](/md/blog.033.png)

图5-13学生提题管理界面

## 5.4教师个人信息、功能模块

教师对个人资料管理信息进行添加、查看、修改以及删除等操作。程序成效图如下图5-14所示：

![](/md/blog.034.png)

图5-14教师功能界面

### 5.4.1文件模板管理
教师对系统文件模板管理进行添加、查看、修改以及删除等操作查看等操作。程序效果图如下图5-15所示：

![](/md/blog.035.png)

图5-15文件模板管理界面

### 5.4.2在线选题管理
教师对在线选题管理信息进行添加、查看、修改以及删除等操作。程序效果图如下图5-16所示：

![](/md/blog.036.png)

图5-16在线选题管理界面


### 5.4.3开题报告管理
教师对开题报告管理信息进行查看编辑课题题目、学生学号、教师工号、提交时间等操作。程序效果图如下图5-17所示：

![](/md/blog.037.png)

图5-17中期报告管理界面

### 5.4.4论文进度管理
教师对论文进度管理信息进行查看编辑课题题目、学生学号、学生姓名、教师工号、提交时间进行添加、查看、修改以及删除等操作。程序效果图如下图5-18所示：

![](/md/blog.038.png)

` `图5-18论文进度管理界面



## 5.5 学生功能模块

学生对个人资料管理信息进行添加、查看、修改以及删除等操作。程序成效图如下图5-19所示：

![](/md/blog.039.png)

图5-19学生功能界面

## 5.5.1学生提问管理
学生对学生提问进行编辑查看添加、修改以及删除等操作等操作。程序效果图如下图5-20所示：

![](/md/blog.040.png)

图5-20学生提问管理界面
## 5.5.2老师答疑管理
学生对老师答疑管理进行查看编辑添加、修改以及删除等操作等操作。程序效果图如下图5-21所示：

![](/md/blog.041.png)

图5-21老师答疑管理界面

## 5.5.3 开题报告管理
学生对开题报告管理信息进行查看等操作。程序效果图如下图5-22所示：

![](/md/blog.042.png)

图5-22开题报告管理界面
## 5.5.4学生提题管理
学生对学生提题管理信息进行查看编辑添加、修改以及删除等操作。程序效果图如下图5-23所示：

![](/md/blog.043.png)

图5-23学生提题管理界面
















