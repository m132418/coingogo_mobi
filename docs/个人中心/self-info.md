# 请求个人信息 #
  会检查登陆用户id和请求的客户端是否一致，过了就返回个人信息，否则报错

**url:**

  http://dev2.coingogo.com:10/mobi/member/self-info

**入参:**

      {
       "id": "101",       
       "vcd":"7b88e53ce5482c310989e74157aa7419"
      }

**成功：**


	{
    "state": {
        "cd": 1,
        "msg": "Success"
    },
    "data": {
        "id": 101,
        "username": "coingogo",
        "auth_key": "4hA7SvvUAVXC1xLSfj_f1uJ_OO-nniwt",
        "password_hash": "$2y$13$.WAq.xSIku9X92a.PdOriebtoVqPUPYnm8ux9SHHFcxFKgDsvN9Fi",
        "password_reset_token": "",
        "email": "admin@admin.com",
        "mobile": "23322024541",
        "avatar": "n5c4h8GKMXPGGY6Jt1sovDpKPKhQ7VXz.jpg",
        "notification_count": 0,
        "role": 20,
        "vip": 0,
        "status": 10,
        "article_status": 0,
        "created_at": 1459842295,
        "updated_at": 1515555035,
        "tx_password_hash": null,
        "mail_verify": 0,
        "pid": 0,
        "signature": "",
        "email_hash": null
    }
	}


**失败:**
    
有两种情况1是没登陆2是对不上客户端 

       {
    "state": {
    "cd": -1,
    "msg": "请先登陆"
    	}
    	}
 