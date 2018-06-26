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


**baidu mqtt api**

|位置|路由|更新视图|测试通过|
|:------|：------|:-------|:------|
|mqtt/cmd/|MqttMessageView|||
|/schedule/tasks.py||||
|
