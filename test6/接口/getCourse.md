# 接口：getCourse  [返回](../README.md)
用例：[老师选课](../example/老师选课.md)， [学生选课](../example/学生选课.md)

- 权限：
    学生：必须老师选课后学生才可以选课。

- 功能：
    返回课程列表。

- API请求地址：
   接口基本地址/v1/api/getCourse/<term_id>

- 请求方式 ：
    GET

- 请求参数说明:
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |term_id|学期编号|
- 返回实例：
```
        {
            "status": true,
            "info": null,
            "total": 10,
            "data": [
                {
                "COURSE_ID": "01",
                "COURSENAME": "软件系统分析与设计技术",
                },
                {
                ...其他课程
                }
            ]
        }
```
- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |total|返回课程总数|
  |data|所有课程的数组|
  |COURSE_ID|课程编号|
  |COURSENAME|课程名字|