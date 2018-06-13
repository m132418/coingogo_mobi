检查post过来手机号是否合法的手机号，是否已经被注册过 ，如果可以注册就发注册验证码

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

并且注册手机收到注册验证码,否则返回错误信息。
需要注意的是一个号一天只能发5个短消息,而且收到验证码一分钟内注册使用。


拿到注册短信进行注册,根据原型图，uname就是phone number,所以会以手机号为username 注一个会员

**url:**

http://dev2.coingogo.com:10/mobi/member/reg

入参

    {
       "uname" : "15311678029",
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
    
