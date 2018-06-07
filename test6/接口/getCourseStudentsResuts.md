# 接口：getCourseStudentsResuts  [返回](../README.md)
用例： [查看成绩](../example/查看成绩.md)，[评定成绩](../example/评定成绩.md)

- 功能：
    返回所选具体学期的课程的实验列表。
    
- 权限：    
    学生: 只能查看自己选择的课程
    老师：只能选择自己所教的课程。
    
- API请求地址： 
    接口基本地址/v1/api/getCourseStudentsResuts/<term_id>/<course_id>/<student_id>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |term_id|学期的编号|
  |course_id|课程的编号|
  |student_id|学生的编号|
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
