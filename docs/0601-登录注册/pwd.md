# 先发验证码 #

**url:**

http://dev2.coingogo.com:10/mobi/member/send-chg-cd

**入参:**

	{
		"vcd":"55c53c8d85292bba31d8409bbd88dc58",
		"uid":101,
		"token":"5f571cc6c47b1e57606532892b01e1ed"
	}

**结果：**

如果成功了返回

	{
    "state": {
        "cd": 1,
        "msg": "done"
    	}
	}



# 改登陆pwd #

**url:**

http://dev2.coingogo.com:10/mobi/member/chg-login-pwd

入参

	{
		"vcd":"9d75b745a1b0dfb076fd325115df6726",
		"uid":101,
		"token":"5f571cc6c47b1e57606532892b01e1ed",
		"code":456123,
		"prepwd":"123123123",
		"pwd":"abc123"
	}
    


# 改交易pwd #

**url:**

http://dev2.coingogo.com:10/mobi/member/chg-tx-pwd

入参

	{
		"vcd":"55c53c8d85292bba31d8409bbd88dc58",
		"uid":101,
		"token":"5f571cc6c47b1e57606532892b01e1ed",
		"code":456123,
		"prepwd":"123123123",
		"pwd":"abc123"
	}
    

----------------------------Email--------------------------

# 先发验证码 #

**url:**

http://dev2.coingogo.com/mobi/member/send-email-chg-cd

**入参:**

	{
		"vcd":"55c53c8d85292bba31d8409bbd88dc58",
		"email":"hongss@126.com"
		
	}

**结果：**

如果成功了返回

	{
    "state": {
        "cd": 1,
        "msg": "done"
    	}
	}






# 改登陆pwd #

**url:**

http://dev2.coingogo.com/mobi/member/email-chg-login-pwd

入参

	{
		"vcd":"c9f0d11f9a35fc0a68366ef3ae619db4",
		"email":"tmcn@foxmail.com",
		"code":"APhVqo",		
		"pwd":"123456"
	}
    



# 检测email收到验证码 #

**url:**

http://dev2.coingogo.com/mobi/member/chk-email-vcd

入参

	{
		"vcd":"4c21b99e90e6cff8db5ff635babaa27a",
		"email":"tmcn@foxmail.com",
		"code":"APhVqo"		
	
	}
    