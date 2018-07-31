# 微讯发布 #


**url**

http://dev2.coingogo.com:10/mobi/wei-xun/post

**入参**

	{
		"title":"题目题目涕涕涕",
		"content":"内容随便随便随便拉",
		"vcd":"ac166a36745546782ad77eae4cce326a",
		"uid":101,
		"token":"5f571cc6c47b1e57606532892b01e1ed"
	}

参看新闻评论，app 带上uid和token
须知，先登入不然报错
题目，内容不可为空，如果发布成功了返回如下

	{
	    "state": {
	        "cd": 1,
	        "msg": "done"
	    }
	}