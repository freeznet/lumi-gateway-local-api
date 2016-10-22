# 无线开关传感器


##属性上报

无线开关传感器每按键一次上报一个报文。400ms内按两次上报的报文是双击。

| 属性 | 说明 |
| -- | -- |
| status | click/double_click    (单击/双击) |
| battery | 0-100电池电量 |

```{"cmd":"report","model":"switch","sid":"112316","short_id":4343,"token":"5","data":"{\"status\":\"click\"}" }```

```{"cmd":"report","model":"switch","sid":"112316","short_id":4343,"token":"6","data":"{\"status\":\"double_click\"}" }```

##心跳上报(~60分钟每次)

```{"cmd":"report","model":"motion","sid":"112316","short_id":4343,"token":"4","data":"{\"battery\":\"65\"}" }```



