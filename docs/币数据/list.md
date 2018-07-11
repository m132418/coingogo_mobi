# 币数据列表 #
**url**
http://dev2.coingogo.com:10/mobi/coin/list

入参

	{
	   "assets" : "10000",
	   "name" : "BTC",
	   "price" : "1-100",
		"page" : 0,	   
	   "psize" : 5,	   
	   "token" : "5f571cc6c47b1e57606532892b01e1ed",
	   "uid" : 101,
	   "vcd" : "d69b9047238cb37936f09d1750b750c3"
	}


参数描述
price 

							price="1"  1元以下							
							price="1-100"  1-100元							
							price="100-500"  100-500元							
							price="500-1000"  500-1000元							
							price="1000-5000"  1000-5000元							
							price="5000-10000"  5000-10000元							
							price="10000"  1万元以上
assets 

							assets="10000"  1万以下
							assets="10000-1000000"  1万-1百万
							assets="1000000-10000000"  1百万-1千万
							assets="10000000-50000000"  1千万-5千万
							assets="50000000-100000000"  5千万-1亿
							assets="100000000-1000000000"  1亿-10亿
							assets="1000000000"  10亿以上

name 按照名字过滤；page 当前页 从0 开始，psize 每页 几个记录