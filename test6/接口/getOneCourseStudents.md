<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getOneCourseStudents  [返回](../README.md)

- 功能：
    用于获得一个课程的学生列表
    
- 权限：
    老师：可获得选择课程的学生列表
    
- API请求地址： 
    接口基本地址/v1/api/getOneCourseStudents/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |course_id|课程的编号|
    
- 返回实例：

        {         
            "status": true,
            "info": null,    
            "course_id": "201510315203", 
            "course_name": "java", 
            "student_number": 30,     
            "data": [
                {
                "student_id":1,
                "student_name":"高杰"
                }, 
                {
                ...其他学生
                }
            ] 
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |student_id|学号|
  |student_name|真实姓名|   
  |student_number|总数|



