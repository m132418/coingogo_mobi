# 首页 #

**url:**

http://dev2.coingogo.com:10/mobi/knowledge/ask

**入参**

	{
		"tags":"区块链",
		"category_id":2,
		"content":"地球什么时候秃噜扣?",
		"title":"瞎操心",
		"amount_type":0 , // 悬赏类型  0=源点 1=不悬赏  ;以实际数据库数据 和 原有程序处理为准
		"yuandian":3, //如果amount_type=0 了那么 必须有这个字段
       "vcd":"a2514028d09ac77493942fe1f338b2aa",
	"uid":101,
	"token":"b9a336214e47717c49641e1e3dcf6a61"
	}

**返回略**


# 提高悬赏 #

**url:**

http://dev2.coingogo.com:10/mobi/knowledge/increase-reward

**入参**

	{
	
		"id":5321,		
		"yuandian":3, //如果amount_type=0 了那么 必须有这个字段
       "vcd":"a2514028d09ac77493942fe1f338b2aa",
	"uid":101,
	"token":"b9a336214e47717c49641e1e3dcf6a61"
	}