城市列表获取接口
=====================

获取城市列表
---------------------

URL::

    GET /city/

查询成功响应信息::

    Status:200 OK

    [
            {
            "city_name": "鞍山",
            "city_id": 2922,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "阿拉善盟",
            "city_id": 2923,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "安庆",
            "city_id": 2924,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "安阳",
            "city_id": 2925,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "安顺",
            "city_id": 2926,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "安康",
            "city_id": 2927,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "阿克苏",
            "city_id": 2928,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "安吉",
            "city_id": 2929,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "安丘",
            "city_id": 2930,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "安岳",
            "city_id": 2931,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "安平",
            "city_id": 2932,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "安溪",
            "city_id": 2933,
            "first_char": "A",
            "hot_city": 0
            },
            {
            "city_name": "安宁",
            "city_id": 2934,
            "first_char": "A",
            "hot_city": 0
            }
    ]

总计800余城市，在此略去

响应参数说明

============== ======== ================   
name            type     value
============== ======== ================
city_name      string   城市名称
city_id        int      城市id
first_char     string   城市首字母
hot_city       bool     热门城市标识
============== ======== ================












