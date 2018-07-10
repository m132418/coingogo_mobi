# 更换电邮 #

发送验证码

**url:**

http://dev2.coingogo.com:10/mobi/member/change-email

**入参:**

	{
	"vcd":"27f16261eb3d026cbc73eae907184da2",
	"uid":101,
	"token":"5f571cc6c47b1e57606532892b01e1ed",
	"email":"xxx@foxmail.com"
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

http://dev2.coingogo.com:10/mobi/member/udt-email

入参

	{
	"vcd":"473d2cce8ea0e5c91916224ff67a62a8",
	"uid":101,
	"token":"5f571cc6c47b1e57606532892b01e1ed",
	"email":"xxx@foxmail.com",
	"code":"mD8Rxt"
	}
    
如果成功返回：
    

	{
	    "state": {
	        "cd": 1,
	        "msg": "Success"
	    }
	}
    
