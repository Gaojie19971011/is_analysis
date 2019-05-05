<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setCourse  [返回](../README.md)
用例： [选择课程](../用例/setCourse.md)

- 功能：
    选择课程

- 权限：
    学生/老师：选择自己的课程，老师选完学生才能选，必须先登录。

- API请求地址：
    接口基本地址/v1/api/setCourse

- 请求方式 ：
    POST

- 请求实例：

        {
            "Course_id":1234,
            "userID":154564
        }

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |user_id|用户的ID号。对应表USERS.USER_ID的值|
  |course_id|课程的编号|

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


