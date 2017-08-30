|类型|url|说明|备注|
|-|-|-|-|
|乐购-进入							|https://api.qdingnet.com/qding-api/api/json/legou-goods/selGoodsBySort 获取乐购商品列表信息							|			ui		|
|乐购-切换	category				|https://api.qdingnet.com/qding-api/api/json/legou-goods/selGoodsBySort 获取乐购商品列表信息							|			ui(点击)|
|乐购-点购物车						|https://api.qdingnet.com/qding-api/api/json/legou-order/getCarts  获取购物车列表										|					ui|
|乐购-添加购物车					|https://api.qdingnet.com/qding-api/api/json/legou-goods/selGoodsDetails  获取商品详情									|				ui|
|								|https://api.qdingnet.com/qding-api/api/json/legou-order/addCart  加入购物车												|			ui|
|乐购-设置							|https://api.qdingnet.com/qding-api/api/json/notify/getNotifySettings  												|			ui|
|乐购-帖子评论/赞					|https://api.qdingnet.com/qding-api/api/json/neighbor/getHistoryNotifysByMId  获取用户历史被点赞，评论消息列表				|				ui|
|乐购-点击帖子						|https://api.qdingnet.com/qding-api/api/json/neighbor/getTopicDetail  获取话题详情									|				ui|
|								|https://api.qdingnet.com/qding-api/api/json/neighbor/getCommentsBytopicId  分页获取评论信息列表							|				ui|
|乐购-帖子-loadmore				|https://api.qdingnet.com/qding-api/api/json/neighbor/getCommentsBytopicId  分页获取评论信息列表							|					ui(点击)|
|乐购-发送评论						|https://api.qdingnet.com/qding-api/api/json/neighbor/addComment  分页获取评论信息列表									|			ui|
|乐购-系统消息						|https://api.qdingnet.com/qding-api/api/json/notify/getSysNotifies													|		ui|
|乐购-管家提醒						|https://api.qdingnet.com/qding-api/api/json/notify/getBusinessNotifies												|			ui|
|乐购-点击商品详情					|https://api.qdingnet.com/qding-api/api/json/legou-goods/selGoodsDetails  获取商品详情									|			ui|
|								|https://api.qdingnet.com/qding-api/api/json/legou-goods/getWareCommentList  获取订单评价列表								|				ui|
|乐购-详情-点击购物车				|https://api.qdingnet.com/qding-api/api/json/legou-order/getCarts  获取购物车列表											|				ui|
|								|https://api.qdingnet.com/qding-api/api/json/legou-order/getPromotionInfoForCart  获取当前购物车中获取所优惠信息				|				ui|
|乐购-详情-购物车-选中/取消			|https://api.qdingnet.com/qding-api/api/json/legou-order/getPromotionInfoForCart  获取当前购物车中获取所优惠信息				|	ui|
|乐购-购物车-点结算					|https://api.qdingnet.com/qding-api/api/json/legou-order/confirmOrder  确定订单										|			ui|
|								|https://api.qdingnet.com/qding-api/api/json/legou-order/getInvoicesByMid  获取用户发票信息列表							|					ui|
|乐购-购物车-点支付					|https://api.qdingnet.com/qding-api/api/json/legou-order/makeOrder  下单（生成订单）									|				ui|
|								|https://api.qdingnet.com/qding-api/api/json/payment/getPayMethod  收银台												|					ui|
|乐购-我的-我的订单					|https://api.qdingnet.com/qding-api/api/json/legou-order/getBusinessListByMemberId  获取当前用户下过订单的业态			|			ui|
|								|https://api.qdingnet.com/qding-api/api/json/legou-order/getOrders   获取订单列表，新增多业态订单							|				ui|
|								|https://api.qdingnet.com/qding-api/api/json/legou-order/getOrderStatus   批量获取多业态订单状态							|				ui|
|乐购-我的订单-兑换码				|https://api.qdingnet.com/qding-api/api/json/legou-order/getRedeemCodeOrders  获取兑换码列表								|				ui|
|门禁卡							|https://api.qdingnet.com/qding-api/api/json/entrance-card/list   门禁卡管理列表											|				ui|
|门禁卡-开卡						|https://api.qdingnet.com/qding-api/api/json/entrance-card/bindAuth 用户开卡鉴权											|				ui|
|门禁卡-验证						|https://api.qdingnet.com/qding-api//api/json/entrance-card/bindAuth  用户开卡鉴权										|			ui|
|门禁卡-检测						|https://api.qdingnet.com/qding-api//api/json/entrance-card/isNewCard 检测门禁卡											|				ui|
|								|https://api.qdingnet.com/qding-api//api/json/entrance-card/settingForNew  门禁卡管理列表									|			ui|
|								|https://api.qdingnet.com/qding-api//api/json/entrance-card/settingForUpdate  门禁卡管理列表								|			ui|
|门禁卡-修改						|https://api.qdingnet.com/qding-api//api/json/entrance-card/newSave   新保存												|			ui(点击)|
|								|https://api.qdingnet.com/qding-api//api/json/entrance-card/updateSave   更新											|				ui(点击)|
|								|https://api.qdingnet.com/qding-api//api/json/entrance-card/renewal  重新激活												|			ui(点击)|
|								|https://api.qdingnet.com/qding-api//api/json/entrance-card/close 消卡													|			ui(点击)|
|								|https://api.qdingnet.com/qding-api//api/json/entrance-card/active  激活													|			ui(点击)|








 

####乐购-进入						

	https://api.qdingnet.com/qding-api/api/json/legou-goods/selGoodsBySort 获取####乐购商品列表信息							 			ui		 

####乐购-切换	category	
	https://api.qdingnet.com/qding-api/api/json/legou-goods/selGoodsBySort 获取####乐购商品列表信息							 			ui(点击) 

####乐购-点购物车					

	https://api.qdingnet.com/qding-api/api/json/legou-order/getCarts  获取购物车列表										 					ui 

####乐购-添加购物车					

	https://api.qdingnet.com/qding-api/api/json/legou-goods/selGoodsDetails  获取商品详情									 				ui 

	https://api.qdingnet.com/qding-api/api/json/legou-order/addCart  加入购物车												 			ui 

####乐购-设置						

	https://api.qdingnet.com/qding-api/api/json/notify/getNotifySettings  												 			ui 

####乐购-帖子评论/赞					

	https://api.qdingnet.com/qding-api/api/json/neighbor/getHistoryNotifysByMId  获取用户历史被点赞，评论消息列表				 				ui 

####乐购-点击帖子					

	https://api.qdingnet.com/qding-api/api/json/neighbor/getTopicDetail  获取话题详情									 				ui 

	https://api.qdingnet.com/qding-api/api/json/neighbor/getCommentsBytopicId  分页获取评论信息列表							 				ui 

####乐购-帖子-loadmore				

	https://api.qdingnet.com/qding-api/api/json/neighbor/getCommentsBytopicId  分页获取评论信息列表							 					ui(点击) 

####乐购-发送评论					

	https://api.qdingnet.com/qding-api/api/json/neighbor/addComment  分页获取评论信息列表									 			ui 

####乐购-系统消息					

	https://api.qdingnet.com/qding-api/api/json/notify/getSysNotifies													 		ui 

####乐购-管家提醒					

	https://api.qdingnet.com/qding-api/api/json/notify/getBusinessNotifies												 			ui 

####乐购-点击商品详情					

	https://api.qdingnet.com/qding-api/api/json/legou-goods/selGoodsDetails  获取商品详情									 			ui 

	https://api.qdingnet.com/qding-api/api/json/legou-goods/getWareCommentList  获取订单评价列表								 				ui 

####乐购-详情-点击购物车				

	https://api.qdingnet.com/qding-api/api/json/legou-order/getCarts  获取购物车列表											 				ui 

	https://api.qdingnet.com/qding-api/api/json/legou-order/getPromotionInfoForCart  获取当前购物车中获取所优惠信息				 				ui 

####乐购-详情-购物车-选中/取消			

	https://api.qdingnet.com/qding-api/api/json/legou-order/getPromotionInfoForCart  获取当前购物车中获取所优惠信息				 	ui 

####乐购-购物车-点结算				

	https://api.qdingnet.com/qding-api/api/json/legou-order/confirmOrder  确定订单										 			ui 

	https://api.qdingnet.com/qding-api/api/json/legou-order/getInvoicesByMid  获取用户发票信息列表							 					ui 

####乐购-购物车-点支付				

	https://api.qdingnet.com/qding-api/api/json/legou-order/makeOrder  下单（生成订单）									 				ui 

	https://api.qdingnet.com/qding-api/api/json/payment/getPayMethod  收银台												 					ui 

####乐购-我的-我的订单				

	https://api.qdingnet.com/qding-api/api/json/legou-order/getBusinessListByMemberId  获取当前用户下过订单的业态			 			ui 

	https://api.qdingnet.com/qding-api/api/json/legou-order/getOrders   获取订单列表，新增多业态订单							 				ui 

	https://api.qdingnet.com/qding-api/api/json/legou-order/getOrderStatus   批量获取多业态订单状态							 				ui 

####乐购-我的订单-兑换码				

	https://api.qdingnet.com/qding-api/api/json/legou-order/getRedeemCodeOrders  获取兑换码列表								 				ui 

####门禁卡							

	https://api.qdingnet.com/qding-api/api/json/entrance-card/list   ####门禁卡管理列表											 				ui 

####门禁卡-开卡						

	https://api.qdingnet.com/qding-api/api/json/entrance-card/bindAuth 用户开卡鉴权											 				ui 

####门禁卡-验证						

	https://api.qdingnet.com/qding-api//api/json/entrance-card/bindAuth  用户开卡鉴权										 			ui 

####门禁卡-检测						

	https://api.qdingnet.com/qding-api//api/json/entrance-card/isNewCard 检测####门禁卡											 				ui 

	https://api.qdingnet.com/qding-api//api/json/entrance-card/settingForNew  ####门禁卡管理列表									 			ui 

	https://api.qdingnet.com/qding-api//api/json/entrance-card/settingForUpdate  ####门禁卡管理列表								 			ui 

####门禁卡-修改						

	https://api.qdingnet.com/qding-api//api/json/entrance-card/newSave   新保存												 			ui(点击) 

	https://api.qdingnet.com/qding-api//api/json/entrance-card/updateSave   更新											 				ui(点击) 

	https://api.qdingnet.com/qding-api//api/json/entrance-card/renewal  重新激活												 			ui(点击) 

	https://api.qdingnet.com/qding-api//api/json/entrance-card/close 消卡													 			ui(点击) 

	https://api.qdingnet.com/qding-api//api/json/entrance-card/active  激活													 			ui(点击) 
