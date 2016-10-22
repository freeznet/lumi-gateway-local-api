# 门窗传感器

##属性上报

(~60分钟每次),窗磁传感器贴在窗户上或门上感知窗户的状态，每动作一次发送一次report。

| 属性 | 说明 |
| -- | -- |
| status | open/close  (开/关) |
| battery | 0-100电池电量 |

```{"cmd":"report","model":"magnet","sid":"89234324","short_id":4343,"token":"3","data":"{\"status\":\"open\"}" }```

##心跳上报

```{"cmd":"report","model":"motion","sid":"89234324","short_id":4345,"token":"4","data":"{\"battery\":\"62\"}" }```

magnet代码是窗磁， 89234324代表的设备的ID（64位的长16进制字符串），status 是窗磁的开关状态,token是一个变化的字符串（不用管这个字段）。





