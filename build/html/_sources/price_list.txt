场次及票价列表获取接口
=========================

获取场次票价列表
-------------------------

URL::

    GET /ticket/

请求参数说明

======================= ========== ==================
name                     type       value
======================= ========== ==================
city_id                 int         查询城市ID   
meituan_moive_id        string      查询电影美团ID
meituan_cinema_id       string      查询电影院美团ID
nuomi_movie_id          string      查询电影糯米ID
nuomi_cinema_id         string      查询电影院糯米ID
taobao_movie_id         string      查询电影淘宝ID
taobao_cinema_id        string      查询电影院淘宝ID
======================= ========== ==================

查询成功响应信息::

    Status: 200 OK

    [
        [],
        {
        "nuomi_now_price": "44",
        "taobao_now_price": "22",
        "start_time": "10:00",
        "end_time": "11:33",
        "meituan_now_price": "33"
        },
        {
        "nuomi_now_price": "44",
        "taobao_now_price": "22",
        "start_time": "11:00",
        "end_time": "12:33",
        "meituan_now_price": "33"
        },
        {
        "nuomi_now_price": "44",
        "taobao_now_price": "22",
        "start_time": "11:45",
        "end_time": "13:18",
        "meituan_now_price": "33"
        },
        {
        "nuomi_now_price": "44",
        "taobao_now_price": "22",
        "start_time": "12:45",
        "end_time": "14:18",
        "meituan_now_price": "33"
        }
    ]
  
响应参数说明

=================== ============ =================
name                 type         value
=================== ============ =================
start_time           string       开始时间
end_time             string       结束时间
meituan_now_price    string       美团现价
nuomi_now_price      string       糯米现价
taobao_now_price     string       淘宝现价
=================== ============ =================

查询失败响应

以下HTTP状态码均应为400

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










