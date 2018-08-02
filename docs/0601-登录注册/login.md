# 登陆 #

**url:**

  http://dev2.coingogo.com:10/mobi/member/login

**入参:**
uname/手机号都可以登陆

      {
       "uname" : "coingogo",
       "pwd" : "123456",
       "vcd":"7b88e53ce5482c310989e74157aa7419"
      }

*uname 账户或者手机号；pwd 密码*

**成功：**

     {
    "state": {
        "cd": 1,
        "msg": ""
    	},
    "data": {
        "id": "101",
        "username": "coingogo",
	 "password_hash": "$2y$13$.WAq.xSIku9X92a.PdOriebtoVqPUPYnm8ux9SHHFcxFKgDsvN9Fi",
        "mobile": "23322024541",
        "avatar": "n5c4h8GKMXPGGY6Jt1sovDpKPKhQ7VXz.jpg"
    	}
	}


avatar 头像图片

你下次请求如果需要提供uid ，比如这次 101 附上token，其中token
=md5( password_hash + id)

**失败:**
    
    {
    "state": {
        "cd": -1,
        "msg": "登陆失败"
    	}
	}
 



# 登陆 2#
这个 是验证uid token的，每次启动app 自动调用，验证通过视同登陆.如果对不上就跳转到登陆页面 重新登陆就是了.

**url:**

  http://dev2.coingogo.com:10/mobi/member/login2

**入参:**

      {
       "uid" : 101,
       "token" : "cd0a1f4e44991fdd7c17db3fdc35ad2c",
       "vcd":"0f971354a76ef3b602971a03dae1ae33"
      }

