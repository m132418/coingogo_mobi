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
		"pwd":"abc123"
	}
    
