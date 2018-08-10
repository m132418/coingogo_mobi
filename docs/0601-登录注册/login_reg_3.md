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
		"unionid":"olngMwl6t5mSfTmUDYNGwiscnKYA",
		"openid":"olngMwl6t5mSfTmUDYNGwiscnKYA"	 
	}
    
*source "weixin"第三方标识 微信 "qq" qq ；source_id 第三方登录提供的唯一标识.*


# 三方微信注册 #

**url:**

http://dev2.coingogo.com:10/mobi/member/auth-reg

入参

    {
	   "source" : "weixin",
	   "source_id" : "olngMwl6t5mSfTmUDYNGwiscnKYA",
		"unionid":"olngMwl6t5mSfTmUDYNGwiscnKYA",
		"openid":"olngMwl6t5mSfTmUDYNGwiscnKYA",
       "uname" : "xxx",
       "email" : "mail126@sss.com",
       "pwd":"123456",		
		"mobile":"15321856958",		     
       "vcd":"e215dc8270239f32a433a172054172c4"
    }
    


# 三方微信绑定已有账号 #
**url:**

http://dev2.coingogo.com:10/mobi/member/auth-bing-wx

入参

    {
	   "source" : "weixin",
	   "source_id" : "olngMwl6t5mSfTmUDYNGwiscnKYA",
		"unionid":"olngMwl6t5mSfTmUDYNGwiscnKYA",
		"openid":"olngMwl6t5mSfTmUDYNGwiscnKYA",
       "uname" : "xxx",      
       "pwd":"123456",	     
       "vcd":"e215dc8270239f32a433a172054172c4"
    }