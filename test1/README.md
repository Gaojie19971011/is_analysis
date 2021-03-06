## 实验1 业务流程建模 
- 本实验的目的是了解PlantUML标准，搭建系统分析文档编写平台，并能绘制出一些简单的业务流程。
- 重新绘制Page107图6.1: 考试及成绩管理流程
- 重新绘制Page108图6.2: 客户维修服务流程
- 重新绘制的两个流程图要汇总到REMADE.md文本文件中进行说明，说明文件用Markdown格式编写。

图6.1,代码：
```
@startuml
title <期末考试流程>

|教务处|
:安排考试;
:考试安排表]
|教师|
:出卷;
split
:A、B试卷]

split again
:打印审批表]
|系主任|
:审批签字;
:打印审批表]
end split
 |教务处|
 :打印试卷;
 :试卷]
|学生|
:参加考试;
:答卷]
|教师|
:阅卷出成绩;
fork
:答卷]
:装订成档;
fork again
|教师|
:成绩单]
|教务处|
if (有不合格？) then (有)
 :安排补考;
 fork
 :补考安排表]
 detach
 fork again
 end fork
else
stop
endif
end fork
|教师|
:期末流程结束;
@enduml
```
运行结果：
![](./finalExamProcess.png)


图6.2，代码：
```
@startuml

|客户|
start
:申请服务;
|业务经理|
if (是新客户嘛？) then (是)
:登录客户信息;
else (不是)
endif
:上门勘察;
:制定方案;
|客户|
if (满意吗？) then(否)
stop
else (是)
:签订服务合同;
endif
|业务经理|
fork
:安排工人;
fork again
:安排材料;
end fork
:填写派工单;
|工人|
:领取材料;
:上门服务;
|客户|
:验收并填写反馈意见;
|业务经理|
:教会派工单;
|财务人员|
:结算收款;
stop
@enduml
```
运行结果：
![](./clientRepairSurviceProcess.png)
