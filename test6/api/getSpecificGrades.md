# 接口名称：getSpecificGrades [返回](../README.md)

用例： [学生查看具体成绩](../usecase/workdtlScore.md)

- 功能：
    通过成绩id查询成绩表中的具体各项得分。
   
- API请求地址： 
    接口基本地址/v1/api/getSpecificGrades

- 请求方式 ：
    GET  

- 请求参数说明:        
    请求参数为：gradesId，通过grades查找具体的得分项数据。
    
- 返回实例：

        {
            "status": true,
            "result_specific"：{
                ["程序UI界面",20]
                ["程序可运行度",40]
                ["程序代码复杂度",20]
            }
        }
  
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |result_specific|数组类型，数组中第一个值表示单项打分的要求，第二个值为单项得分|