	# 发帖 #
	
	
	**url:**
	
	http://dev2.coingogo.com/mobi/article/post
	
	**入参:**
	
			{
			   "catid":5,
 				"level":0, //帖子等级（0=>免费 1=>会员 2=>付费）2时候 必须跟个price
				"price":3,
			    "title":"题目1",
			     "content":"题目1的内容",
  				"tags":"区块链技术,代币",
		       "vcd":"a3434651969e147f0b0eba590e838533",
		"uid":101,
		"token":"5f571cc6c47b1e57606532892b01e1ed"
		    	
			}
	
	
没有uid 也能返回必要的数据.

# 拽一些标签供发帖用 #

http://dev2.coingogo.com/mobi/article/pull-tags

	{	
		"howmany":3, 
       "vcd":"e05ddb13ae33d10a58393fc07f9450b9"      
	}



	# 存成草稿 #
	
	
	**url:**
	
	http://dev2.coingogo.com/mobi/article/draft
	
	**入参:**
	
			{
			   "catid":5,
 				"level":0, //帖子等级（0=>免费 1=>会员 2=>付费）2时候 必须跟个price
				"price":3,
			    "title":"题目1",
			     "content":"题目1的内容",
  				"tags":"区块链技术,代币",
		       "vcd":"a3434651969e147f0b0eba590e838533",
		"uid":101,
		"token":"5f571cc6c47b1e57606532892b01e1ed"
		    	
			}



**url:**
	
	http://dev2.coingogo.com/mobi/article/draft-list
	
	**入参:**
	
			{	
	   "page" : 1,
	   "psize" : 5,						
		 "vcd":"2ebd2a8ac3ade1483959e1bcf524c3eb",
		"uid":101,
		"token":"5f571cc6c47b1e57606532892b01e1ed"		    	
			}


**url:**
	
	http://dev2.coingogo.com/mobi/article/draft-view
	
	**入参:**
	
			{							
		 "vcd":"f95138ad60cf6e516c0393217324e20e",
		"uid":101,
		"token":"5f571cc6c47b1e57606532892b01e1ed"	,
		"topicid":4017	    	
			}