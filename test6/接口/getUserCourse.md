<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getUserCourse  [返回](../README.md)

- 功能：
    返回当前用户所有课程
    
- 权限：
    只能看自己的课程
    
- API请求地址： 
    接口基本地址/v1/api/getUserCourse/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |course_id|课程的编号|
  |student_id|学生的学号|
    
- 返回实例：

        {         
            "status": true,
            "info": null,    
            "course_number":6
            "student_id":"201610414204",      
            "data": [
                {
                "course_id":"201610414207"
                }, 
                {
                ...其他课程
                }
            ] 
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |student_id|学号|
  |course_id|课程编号|
  |course_number|课程数量|



