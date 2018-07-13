# 交易所列表 #
**url**
http://dev2.coingogo.com:10/mobi/exchanges/list

入参

	
	{
	   "trade_type" : "狗狗币",
	   "name" : "BTC",
	   "trade_price" : "BitCoin",
		"page" : 0,	   
	   "psize" : 5,	   
	   "vcd" : "859302de9887cfe510995eee5720a269"
	}
	


参数描述
trade_type 

									 trade_type="Bitcoin" 比特币
									 trade_type="Litecoin" 莱特比
									 trade_type="Dogecoin" 狗狗币
									 trade_type="Ethereum" 以太坊
									 trade_type="Ethereum Classic" 以太经典
trade_price

								
								trade_price="cny"
								trade_price="usd"
								trade_price="BitCoin"


name 按照名字过滤；page 当前页 从0 开始，psize 每页 几个记录