## 获取token
--------------------

**简要描述：** 

- 获取token

**请求URL：** 
- `http://{HOST}/api/token.ashx`
  
**请求方式：**
- POST

**参数：** 

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|organize_id    |是  |string |组织id   |
|secret    |否  |string |密钥   |

**请求示例**

- POST `http://{HOST}/api/token.ashx`

``` json
{
    "organize_id": "6731de76-14a6-49ae-97bc-6eba6914391e",
    "secret": "X2PNo9bpM0uEihUPzyrh"
}
```

**返回示例**

``` json
200 OK
Content-type: application/json

{
    "Token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJ...",
    "Expire_In": "3600"//有效时长
}
```

---

**备注：** 