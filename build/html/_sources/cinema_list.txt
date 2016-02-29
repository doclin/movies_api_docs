电影院列表获取接口
====================

获取电影院列表
--------------------

:: 
  GET /cinema/

请求参数说明

==================== =========== ===================
name                  type         value
==================== =========== ===================
city_id              int         所查询城市ID
meituan_movie_id     string      查询电影美团ID
meituan_district_id  string      查询行政区美团ID
nuomi_movie_id       string      查询电影糯米ID
nuomi_district_id    string      查询行政区糯米ID
taobao_movie_id      string      查询电影淘宝ID
taobao_district_id   string      查询行政区淘宝ID
==================== =========== ===================

查询成功响应信息

::
  Status: 200 OK

::
  [
    [],
    {
    "taobao_cinema_id": "",
    "nuomi_cinema_id": "",
    "meituan_cinema_id": "6136366",
    "cinema_name": "CGV星聚汇影城光谷店"
    },
    {
    "taobao_cinema_id": "",
    "nuomi_cinema_id": "",
    "meituan_cinema_id": "85361325",
    "cinema_name": "博纳影城店"
    },
    {
    "taobao_cinema_id": "29670",
    "nuomi_cinema_id": "e3513addc51f7e803ce23137",
    "meituan_cinema_id": "67477397",
    "cinema_name": "东澜岸天河影城"
    },
    {
    "taobao_cinema_id": "18994",
    "nuomi_cinema_id": "",
    "meituan_cinema_id": "1474786",
    "cinema_name": "光谷正华银兴影城"
    },
    {
    "taobao_cinema_id": "5609",
    "nuomi_cinema_id": "",
    "meituan_cinema_id": "1476216",
    "cinema_name": "洪山天河影城"
    },
    {
    "taobao_cinema_id": "13796",
    "nuomi_cinema_id": "231375a34427680cf8dc85e2",
    "meituan_cinema_id": "6928505",
    "cinema_name": "华夏影城鲁广店"
    },
    {
    "taobao_cinema_id": "7283",
    "nuomi_cinema_id": "",
    "meituan_cinema_id": "1439523",
    "cinema_name": "华谊兄弟影院光谷店"
    },
    {
    "taobao_cinema_id": "9801",
    "nuomi_cinema_id": "893a52349e89495788db73a6",
    "meituan_cinema_id": "2410366",
    "cinema_name": "巨幕影城光谷广场资本大厦店"
    },
    {
    "taobao_cinema_id": "25691",
    "nuomi_cinema_id": "44c910d034e0e06ebea24038",
    "meituan_cinema_id": "4629797",
    "cinema_name": "天河欢乐汇影城"
    },
    {
    "taobao_cinema_id": "",
    "nuomi_cinema_id": "",
    "meituan_cinema_id": "4267320",
    "cinema_name": "幸福蓝海影城雄楚店"
    },
    {
    "taobao_cinema_id": "21299",
    "nuomi_cinema_id": "",
    "meituan_cinema_id": "42024070",
    "cinema_name": "银兴菲林影城佰港城店"
    },
    {
    "taobao_cinema_id": "7961",
    "nuomi_cinema_id": "",
    "meituan_cinema_id": "1439056",
    "cinema_name": "中影影城光谷天河店"
    },
    {
    "taobao_cinema_id": "28672",
    "nuomi_cinema_id": "",
    "meituan_cinema_id": "51041148",
    "cinema_name": "耀莱成龙影城"
    }

  ]

响应参数说明

===================== =========== ==================
name                  type        value
===================== =========== ==================
cinema_name           string      电影院名称
meituan_cinema_id     string      查询影院美团ID
nuomi_cinema_id       string      查询影院糯米ID
taobao_cinema_id      string      查询影院淘宝ID
===================== =========== ==================

查询失败响应

以下HTTP状态码均应为400

1.city_id格式正确但不存在该ID

::
  {
  "message": "Id dose not exist"
  }

2.请求参数格式错误

::
  {
  "city_id": ["invalid"]
  }

3.其他错误

::
  {
  "message": "Unknown error"
  }







