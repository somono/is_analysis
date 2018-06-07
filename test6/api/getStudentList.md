# 接口：getStudentList [返回](../README.md)

用例： [学生列表](../usecase/studentList.md)

- 功能： 返回该实验所有学生的列表。
    
- API请求地址： 
   接口基本地址/v1/api/getStudentList

- 请求方式 ：
    GET  

- 请求参数说明:        
    请求参数为：termId，testId。termId确定学期，testId确定实验，进一步提取学生信息。
    
- 返回实例：

        {
            "status": true,
            "studentList":{
                ["2016104312"，"张三"，"zzz"],
                ["2016104313"，"李四"，"zzz"]，
                ["2016104314"，"王五"，"zzz"]，
                ...
            }
        }
  
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |studentList|返回所有该实验的学生信息|