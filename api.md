**1.国内单基站查询接口**

查询全国移动联通电信2G/3G/4G基站位置数据

接口地址：https://www.findlbs.com/cell

请求示例:  https://www.findlbs.com/cell?mcc=460&mnc=0&lac=20616&ci=220100352

| 名称 | 类型 | 必填 | 说明                                            |
| ---- | ---- | ---- | ----------------------------------------------- |
| mcc  | int  | 是   | mcc国家代码：中国代码 460                       |
| mnc  | int  | 是   | mnc网络类型：0移动，1联通 (电信对应sid)，十进制 |
| lac  | int  | 是   | lac (电信对应nid)，十进制                       |
| ci   | int  | 是   | cellid (电信对应bid)，十进制                    |

返回数据格式：JSON

{
    "code": 0,
    "message": "ok",
    "latitude": 34.632502,
    "longitude": 112.505417,
    "address": "河南省洛阳市洛龙区伊洛路"
}

<br>
<br>

#### **2.国内单WIFI查询接口**

查询全国WIFI热点位置数据

接口地址：https://www.findlbs.com/wifi

请求示例: https://www.findlbs.com/wifi?mac=30:fc:68:2a:0e:1c

请求参数:

| 名称 | 类型   | 必填 | 说明                      |
| ---- | ------ | ---- | ------------------------- |
| mac  | string | 是   | WIFI热点的MAC地址 (BSSID) |

返回数据格式：JSON

0: 成功

{
    "code": 0,
    "message": "ok",
    "latitude": 36.176407,
    "longitude": 120.42575,
    "address": "山东省青岛市李沧区金水路1014号"
}


[![HitCount](https://hits.dwyl.com/findlbs/lbsdata.svg?style=flat)](http://hits.dwyl.com/findlbs/lbsdata)
