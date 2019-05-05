<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setSemmester  [返回](../README.md)
用例： [选择课程](../用例/setSemester.md)

- 功能：
    设置学期
      
    
- API请求地址： 
    接口基本地址/v1/api/setSemester

- 请求方式 ：
    POST

- 请求实例：

        {
            "semester_id":"大一上学期"

        }
        
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |semester_id|课程的编号| 
  
- 返回实例：

        {         
            "status": true,
            "info": null,    

        }
 
- 返回参数说明： 
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|


