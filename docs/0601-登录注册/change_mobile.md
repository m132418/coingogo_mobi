# 更换手机号 #

发送验证码

**url:**

http://dev2.coingogo.com:10/mobi/member/change-mobile

**入参:**

	{
	"vcd":"27f16261eb3d026cbc73eae907184da2",
	"uid":101,
	"token":"5f571cc6c47b1e57606532892b01e1ed",
	"mobile":"13356585698"
	}

**结果：**

如果成功了返回

	{
    "state": {
        "cd": 1,
        "msg": "Success"
    	}
	}	



# 收到码字更换 #


**url:**

http://dev2.coingogo.com:10/mobi/member/udt-mobile

入参

	{
	"vcd":"a58d9a5e57595c7438a5c2129517a39f",
	"uid":101,
	"token":"5f571cc6c47b1e57606532892b01e1ed",
	"mobile":"13356585698",
	"code":"433846"
	}
    
如果成功返回：
    

	{
	    "state": {
	        "cd": 1,
	        "msg": "Success"
	    }
	}
    
