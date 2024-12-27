## 作业

内容：将上次的登录作业接上数据库，并实现注册

一些接口用例

#### 注册 POST /api/register

Request: Application/json

```json
{
    "name":"user name",
    "password":"123456"
}
```

Response

```json
{
    "success":true,
    "data":{
        "msg":"注册成功"
    }
}
```

或者

```json
{
    "success":false,
    "data":{
        "msg":"此用户名已经被注册"
    }
}
```

#### 登录 POST /api/

Request

```json
{
    "name":"example",
    "password":"114514"
}
```

Response

```json
{
    "success":true,
    "data":{
        "msg":"登录成功"
    }
}
```

或者

```json
{
    "success":false,
    "data":{
        "msg":"用户名或密码错误"
    }
}
```

#### 登出 DELETE /api/

**Request**

None

**Response**

```json
{
    "success":true,
    "data":{
        "msg":"成功登出"
    }
}
```

