﻿<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 基于GitHub的实验管理平台的分析与设计

### 成都大学信息科学与工程学院

|学号|班级|姓名|
|:-------:|:-------------: | :----------:|
|201610414204|软件工程二班|高杰|

## 1. 概述
- 基于GitHub的实验管理平台的作用是在线管理实验成绩的Web应用系统。学生和老师的实验内容均存放在GitHUB
页面上。
- 学生的功能主要有：一是设置自己的GitHub用户名，二是查询自己的实验成绩。学生的GitHub用户名是公开的，但成绩不公开。
- 老师的功能主要有：一是批改每个学生的成绩，二是查看每个学生的成绩。
- 老师和学生都能通过本系统的链接方便地跳转到学生的每个GitHUB实验目录，以便批改实验或者查看实验情况。
- 实验成绩按数字分数计算，每项实验的满分为100分，最低为0分。
- 系统自动计算每个学生的所有实验的平均分。
- 在上述基础上实现三单变三多，即单学期单课程单评分项改成多   
## 2. 系统总体结构
![](系统总体结构.png)

界面设计参见：https://Gaojie19971011.github.io/is_analysis/test6/ul/index.html
    
## 3. 用例图设计 [源码](src/UseCase.puml)
![](UseCase.png)

## 4. 类图设计 [源码](src/class.puml)
![](class.png)

## 5. 数据库设计
- ### [参见数据库设计](./数据库设计.md)

## 6. 用例及界面详细设计
- ### [“学生列表”用例](./用例/学生列表.md),[界面](https://gaojie19971011.github.io/is_analysis/test6/ul/index.html)
- ### [“课程选择”用例](./用例/学生列表.md),[界面](https://gaojie19971011.github.io/is_analysis/test6/ul/courseselection.html)
- ### [“课程管理”用例](./用例/课程管理.md),[界面](https://gaojie19971011.github.io/is_analysis/test6/ul/coursemanagement.html)
- ### [“评定成绩”用例](./用例/评定成绩.md),[界面](https://gaojie19971011.github.io/is_analysis/test6/ul/rating.html)
- ### [“查看成绩”用例](./用例/查看成绩.md),[界面](https://gaojie19971011.github.io/is_analysis/test6/ul/viewgrades.html)
- ### [“修改密码”用例](./用例/修改密码.md),[界面](https://gaojie19971011.github.io/is_analysis/test6/updatepassword.html)
- ### [“修改用户信息”用例](./用例/修改用户信息.md),[界面](https://gaojie19971011.github.io/is_analysis/test6/ul/updateuserinformation.html)
- ### [“查看用户信息”用例](./用例/查看用户信息.md),[界面](https://gaojie19971011.github.io/is_analysis/test6/ul/userinformation.html)
- ### [“登出”用例](./用例/登出.md),[界面](https://gaojie19971011.github.io/is_analysis/test6/ul/topmenu.html)
- ### [“登录”用例](./用例/登录.md),[界面](https://gaojie19971011.github.io/is_analysis/test6/ul/login.html)
    