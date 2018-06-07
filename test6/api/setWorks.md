<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：publishTest  [返回](../README.md)
用例： [添加实验](../usecase/addWork.md)

- 功能：
    教师发布新的实验任务。
    
- 权限：
    只有老师能用。  
    
- API请求地址： 
    接口基本地址/v1/api/setWorks

- 请求方式 ：
    POST

- 请求实例：

        {
            "course_id":1,
            "title":"实验1",
            "link":"https://github.com/xxx/test/README.md"
        }
        
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |course_id|实验所属课程的编号|
  |title|实验的标题| 
  |link|实验的详细介绍地址（github）|
  
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

