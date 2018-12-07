    
**简要描述：** 

- 获取注册验证码

**请求URL：** 
- ` http://mdao.chinacloudsites.cn/api/user/SendSms `
  
**请求方式：**
- POST 

**参数：** 

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|Phone    |是  |string |手机号   |


 **返回示例**

``` 
  {
    "Status": true,
	"Message":"",
    "data": []
  }
```

**备注：** 
此接口需要优化：发送短信前先查询该手机号是否已经被注册，如果被注册，返回失败结果，Message中说明原因，不发送短信。


