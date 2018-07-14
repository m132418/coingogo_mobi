# 币数据列表 #
**url**
http://dev2.coingogo.com:10/mobi/coin/grade

入参

	{
	   "post_score" : [ 1, 2, 3, 4 ],
	   "token" : "d91a0e16c2e2642427a392011724d85c",
	   "trans_id" : "11",
	   "uid" : 101,
	   "vcd" : "33d2b4f26b2500574f3bfb36d4758904"
	}



trans_id交易所id

post_score 为四个项目 打分  1-4 分

           speed = $post_score[0];
           up_withdraw_speed = $post_score[1];
           platform_stabilize = $post_score[2];
           experience = $post_score[3];


