# 第三方登陆和注册 #
app直接和三方交互，若成功登陆，携带类型source和标识source_id请一个login接口，如果已经绑定过了返回用户信息，如果没有绑定过返回"fail",接着请一个注册绑定接口。

----------

# 登陆 #

**url:**

  http://dev2.coingogo.com:10/mobi/member/auth-login

**入参:**
source :qq,weixin,weibo
    
	{
	   "source" : "weixin",
	   "source_id" : "olngMwl6t5mSfTmUDYNGwiscnKYA",
	   "vcd":"5e133196c77fb2721e387ec2c624cfa7"
	}
    
*source "weixin"第三方标识 微信 "qq" qq ；source_id 第三方登录提供的唯一标识.*

**成功：**

    
    {
    "state": {
        "cd": 1,
        "msg": ""
    	},

    "data": {
    "id": 7126,
    "username": "GhostPrince",
    "auth_key": "CptFNBDAg4Cx_IfhZZlwu77_qxj7Mpu7",
    "password_hash": "$2y$13$2ogtvCX4rbB2t3Dq65Ah1OgTLj.b29uPETXR0qWEJb7qOkBaWeyym",
    "password_reset_token": null,
    "email": "guiwangzilp@126.com",
    "mobile": "18958122729",
    "avatar": null,
    "notification_count": 0,
    "role": 10,
    "vip": 0,
    "status": 10,
    "article_status": 0,
    "created_at": 1485760009,
    "updated_at": 1485760009,
    "tx_password_hash": null,
    "mail_verify": 0,
    "pid": 0,
    "signature": "",
    "email_hash": null
    	}
   
    }
    

**失败:**

    {
     "state": {
        "cd": -1,
        "msg": "登陆失败"
    	}
    }


----------
# 注册绑定 #


**url:**

http://dev2.coingogo.com:10/mobi/member/send-reg-cd

**入参:**

{
   "phone" : "15311678029",
   "vcd":"4c3a8a05a95c5baea98be122e842afb1"
}

**结果：**

如果成功了返回

    {
     "state": {
        "cd": 1,
        "msg": "done"
    	}
    }


*并且注册手机收到注册验证码,否则返回错误信息。
需要注意的是一个号一天只能发5个短消息,而且收到验证码一分钟内注册使用。
拿到注册短信进行注册.*


**url:**

http://dev2.coingogo.com:10/mobi/member/auth-reg

入参

    {
	   "source" : "weixin",
	   "source_id" : "olngMwl6t5mSfTmUDYNGwiscnKYA",
       "uname" : "xxx",
       "email" : "mail126@sss.com",
       "pwd":"123456",
       "vcode":"896547",
       "vcd":"e215dc8270239f32a433a172054172c4"
    }
    
如果注册成功返回：
    
    {
     "state": {
        "cd": 1,
        "msg": "Success"
    	},
    "data": {
        "username": "15321678022",
        "email": "mail126@ss122s.com",
        "mobile": "15321678022",
        "password_hash": "$2y$13$IyEoM7F/jSMbohGMdDNMO.VsMHjSnMAIu7oOki1/ZCUk8N04r1fVu",
        "auth_key": "zbwNZhUD1COF_5i-0K-p9MCJRpO-uPk0",
        "status": 10,
        "created_at": 1528856056,
        "updated_at": 1528856056,
        "id": 54519
    	}
    }