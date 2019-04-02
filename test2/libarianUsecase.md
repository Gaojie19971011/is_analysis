

**“图书管理”用例流程图源码如下：**
``` 
@startuml
start
:图书管理员;
:登录;
:图书管理;
split
:借书;
if (身份验证) then (符合借书条件)
:同意借出图书;
else (不符合)
:不同意借出图书;
endif
split again
:还书;
if (是否违规) then (是)
:作出罚款;
else(否)
endif
:归还成功;
split again
:图书分类;
end split
stop
@enduml
```

**“图书管理”用例流程图如下：**

![](./finalExamProcess.png)
