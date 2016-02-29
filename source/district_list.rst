行政区列表获取接口
=====================

获取行政区列表
---------------------

URL::

  GET /district/

请求参数说明

====================== ============ ====================
name                    type          value
====================== ============ ====================
city_id                 int          查询城市ID
meituan_movie_id        string       查询电影美团ID
nuomi_movie_id          string       查询电影糯米ID
taobao_movie_id         string       查询电影淘宝ID
====================== ============ ====================

查询成功响应信息::

    Status: 200 OK
    [
        [],
        {
        "district_name": "江岸区",
        "taobao_district_id": "江岸区",
        "nuomi_district_id": "3504-0",
        "meituan_district_id": "jiangqu"
        },
        {
        "district_name": "东西湖区",
        "taobao_district_id": "东西湖区",
        "nuomi_district_id": "3908-0",
        "meituan_district_id": "dongxihuqu"
        },
        {
        "district_name": "洪山区",
        "taobao_district_id": "洪山区",
        "nuomi_district_id": "3390-0",
        "meituan_district_id": "hongshanqu"
        },
        {
        "district_name": "汉阳区",
        "taobao_district_id": "汉阳区",
        "nuomi_district_id": "3494-0",
        "meituan_district_id": "hanyangqu"
        },
        {
        "district_name": "武昌区",
        "taobao_district_id": "武昌区",
        "nuomi_district_id": "3437-0",
        "meituan_district_id": "wuchangqu"
        },
        {
        "district_name": "硚口区",
        "taobao_district_id": "硚口区",
        "nuomi_district_id": "3394-0",
        "meituan_district_id": "kouqu"
        },
        {
        "district_name": "江夏区",
        "taobao_district_id": "江夏区",
        "nuomi_district_id": "6711-0",
        "meituan_district_id": "jiangxiaqu"
        },
        {
        "district_name": "江汉区",
        "taobao_district_id": "江汉区",
        "nuomi_district_id": "3357-0",
        "meituan_district_id": "jianghanqu"
        },
        {
        "district_name": "黄陂区",
        "taobao_district_id": "黄陂区",
        "nuomi_district_id": "",
        "meituan_district_id": "huangpiqu"
        },
        {
        "district_name": "青山区",
        "taobao_district_id": "青山区",
        "nuomi_district_id": "",
        "meituan_district_id": "qingshanqu"
        },
        {
        "district_name": "蔡甸区",
        "taobao_district_id": "蔡甸区",
        "nuomi_district_id": "6710-0",
        "meituan_district_id": "caidianqu"
        },
        {
        "district_name": "新洲区",
        "taobao_district_id": "新洲区",
        "nuomi_district_id": "",
        "meituan_district_id": "xinzhouqu"
        },
        {
        "district_name": "汉南区",
        "taobao_district_id": "",
        "nuomi_district_id": "",
        "meituan_district_id": "hannanqu"
        },
        {
        "district_name": "经济技术开发区",
        "taobao_district_id": "经济技术开发区",
        "nuomi_district_id": "",
        "meituan_district_id": ""
        }
    ]

响应参数说明

===================== ========= ==================
name                   type       value
===================== ========= ==================
district_name          string     行政区名称
meituan_district_id    string     美团行政区id
nuomi_district_id      string     糯米行政区id
taobao_district_id     string     淘宝行政区id
===================== ========= ==================

查询失败响应

以下所有错误响应的HTTP状态码均为400

1.city_id格式正确但不存在该ID::

  {
  "message": "Id dose not exist"
  }

2.请求参数格式错误::

  {
  "city_id": ["invalid"]
  }

3.其他错误::

  {
  "message": "Unknown error"
  }
