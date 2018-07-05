# deye_iot_update
**change baidu thing manage to baidu thing hub**

|更新接口|更新视图|测试通过|
|:------|:------|------|
|/device/activation/|ActivationView|yes|
|/device/loraactivate/|LoRaActivationView|yes|
|/enduser/checkVerCode/|checkVerCode|yes|
|/product/vDevice/|VirtualDeviceActivationView|yes|
|/product/virtual/bind/|VirtualDeviceBindView|yes|
|/accounts/signup/|SignUpView|no|
|/wechat/activate/|WechatDeviceActivate|yes|
|/wechat/bind/|Wechat_Bind|yes|
|/product/device/|DeviceView|yes|
||DeviceCreateSerializer|

## pymongo guide

```
 from pymongo import MongoClient
 
 client = MongoClient('mongodb://admin:mxchip2016mongodb@dds-2ze16a8657ee8b041921-
pub.mongodb.rds.aliyuncs.com:3717/fogcloud_v3_main')   

db.authenticate("admin","mxchip2016mongodb")

db = client.fogcloud_v3_main                                                      
                                                                                          
col = db.client_event

res = col.find({"deviceid":"b72d094c2cc811e88d1700163e03b4d6", "ctimestamp":{"$gte": "1530687600000", "$lt": "1530687660000" }}).sort("ctimestamp")
