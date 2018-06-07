

# 接口：getUserCourses  [返回](../README.md)

用例： [选择课程](../usecase/chooseCourse.md) 
   
- 功能：
    返回该用户所存在课程的课程列表。   
    
- API请求地址： 
    接口基本地址/v1/api/getUserCourses

- 请求方式 ：
    GET  

- 请求参数说明:        
    请求有两个个参数：userId、termId，userId参数为用户Id确定用户信息，以便后台查找该用户的相关数据信息。termId确定学期，进一步筛选课程。
    
- 返回实例：

        {
            "status": true,
            "course"：[
                "c语言程序设计",
                "java面向对象",
                "linux程序设计",
                ...
            ]
        }
  
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |course|数组类型，元素表示课程名称|