## 获取token用户信息

创建于 2021-12-10 / 最近更新于 2022-02-22 / 3760

字体： \[默认\] \[大\] \[更大\]

#### 简要描述

> 获取token用户信息

#### 接口版本

| 版本号 | 制定人 | 制定日期 | 修订日期 |
| --- | --- | --- | --- |
| 1.0.0 | Devil | 2020-10-07 |  |

#### 请求URL

> user/tokenuserinfo

#### 请求方式

> POST

#### 公共参数

| 参数名 | 是否必须 | 类型 | 默认值 | 描述 |
| --- | --- | --- | --- | --- |
| application | 是 | string | web | 请求应用、参考公共中详解 |
| application\_client\_type | 是 | string | pc | 请求客户端、参考公共中详解 |
| token | 否 | string |  | token |

#### 请求参数

```
{
    "token": "312d48bec9978b3b81000d6aa33fdbd4"
}
```

| 参数名 | 是否必须 | 类型 | 描述 |
| --- | --- | --- | --- |
| token | 是 | string | token令牌 |

#### 返回示例

**正确时返回**

```
{
    "msg": "success",
    "code": 0,
    "data": {
        "id": "1",
        "alipay_openid": "",
        "weixin_openid": "",
        "weixin_unionid": "",
        "weixin_web_openid": "",
        "baidu_openid": "",
        "toutiao_openid": "",
        "qq_openid": "",
        "qq_unionid": "",
        "status": "0",
        "token": "6663140f41aafba844276834b3d4b893",
        "username": "qqqqqq",
        "nickname": "",
        "mobile": "",
        "email": "",
        "gender": "0",
        "avatar": "http://d1.shopxo.vip/static/index/default/images/default-user-avatar.jpg",
        "province": "",
        "city": "",
        "birthday": "0",
        "address": "",
        "integral": "0",
        "locking_integral": "0",
        "referrer": "2",
        "plugins_distribution_level": "0",
        "is_delete_time": "0",
        "add_time": "1637831935",
        "upd_time": "1638930509",
        "add_time_text": "2021-11-25 17:18:55",
        "upd_time_text": "2021-12-08 10:28:29",
        "gender_text": "保密",
        "birthday_text": "",
        "mobile_security": "",
        "email_security": "",
        "user_name_view": "qqqqqq"
    }
}
```

**错误时返回**

```
{
    "msg": "error",
    "code": -1,
    "data": []
}
```

#### 返回参数说明 -> data

用户基础数据

#### 备注

> 更多返回错误代码请看首页的错误代码描述