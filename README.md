# API Reference

[TOC]

## 基础说明
- 所有Request使用 HTTP POST

- Request 中所有参数使用 UTF-8 URL Encode.

- 公共参数


|参数名|类型|必填|描述|
|--------|--------|--------|--------|
|token|string|是|Token|
|device_id|string|是|IMEI|
|plat|int|是|平台 `1`IOS `2`android|
|cver|int|是|app版本号（int型）|



- Response


## Login
登录
`http://wx.abc.com/index/login`
### Request
|参数名|类型|必填|描述|
|-|-|-|-|
|phone|String|是|...|
|password|String|是|...|
###Response
|参数名|类型|描述|
|-|-|-|-|
|token|String|token|

####E.G
```
{
	"result":1,
	"data":{
		"token":"abc1234"
	}
}
```
## Tasks
任务单列表
`http://wx.abc.com/index/tasks`
### Request
|参数名|类型|必填|描述|
|-|-|-|-|
|ids|String|否|用`,`分隔的一组ID，如`1,2,3,4`|
|tomorrow|String|否|1表示明天，0或NULL为今天|

`ids`,`tomorrow`不会同时出现。
只有`tomorrow`时，返回明天或今天的全部数据。
只有`ids`时，返回id对应的数据。

###Response
|参数名|类型|描述|
|-|-|-|-|
|tasks|JSONArray of Task|所有订单|

Task:

|参数名|类型|描述|
|-|-|-|-|
|id|String |送餐编号|
|order_id|String |订单编号|
|ordered_on|Long |订餐日期|
|order_amount|Float |订单金额|
|discount|Float |优惠金额|
|order_grand_total|Float |应付金额|
|payment_method|Integer |支付方式...|
|cash|Float |现金支付...|
|client_remark|String |客户备注|
|service_remark|String |客服备注|
|shipping_area|String |派送区域|
|deliver_on|Long |送达时间，Timestamp，按照PHP标准精度为秒。|
|shipping_address|String |地址|
|client_name|String |客户名称|
|client_phone|String |客户电话|
|task_status|String |订单状态：1=未接单；2=已接单；3=配送中；4未送达；5已送达|
|pay_status|String |收款状态,`1`已收款 `0`未收款|
|address_lat|Float |送货坐标，经度|
|address_lng|Float |送货坐标，纬度|
|shalas|Integer |沙拉数|
|cakes|Integer |蛋糕数|
|bread|Integer |面包数|
|sauces|Integer |酱汁数|
|special_needs|Integer |特需，`1`是 `0`否|
|goods|JSONArray of Good |客户名称|

Good:

|参数名|类型|描述|
|-|-|-|-|
|name|String |商品名称|
|count|Integer |商品数量|

####E.G
```
	{
		"result": 1,
		"data": {
			"task":{
				"id": "送餐编号",
				"order_id": "订单编号",
				"ordered_on": 13123123123,
				"order_amount": 10.00,
				"discount": 10.00,
				"order_grand_total": 10.00,
				"payment_method": "支付方式",
				"cash": 10.00,
				"client_remark": "客户备注",
				"service_remark": "客服备注",
				"shipping_area": "派送区域",
				"deliver_on": 13123123123,
				"shipping_address": "地址",
				"client_name": "姓名",
				"client_phone": "1311311313",
				"task_status": 1,
				"pay_status": 1, 
				"address_lat":"",
				"address_lng":"",
				"shalas":3,
				"cakes":3,
				"bread":3,
				"sauces":3,
				"special_needs":1,
				"goods": [{
						"name": "产品名",
						"count": 1
					}, {
						"name": "产品名",
						"count": 2
					}
					......
				]
			}

		}
	}
```
## Accept
接单
### Request
|参数名|类型|必填|描述|
|-|-|-|-|
|id|String|是|ID|

###Response

####E.G
```
{
	"result":1
}
```
## Commit
更改配送状态
### Request
|参数名|类型|必填|描述|
|-|-|-|-|
|id|String|是|ID of Task|
|delivered|Integer|是|`1`已送达 `0`未送达|
|payment|Integer|是|`1`已付款 `0`未付款|
|remark|String|是|备注|

###Response

####E.G
```
{
	"result":1
}
```
## Send SMS
批量发送短信
### Request
|参数名|类型|必填|描述|
|-|-|-|-|
|ids|String|是|用`,`分隔的一组ID，如`1,2,3,4`|

###Response

####E.G
```
{
	"result":1
}
```


## Ship
批量开始配送
### Request
|参数名|类型|必填|描述|
|-|-|-|-|
|ids|String|是|用`,`分隔的一组ID，如`1,2,3,4`|

###Response

####E.G
```
{
	"result":1
}
```
