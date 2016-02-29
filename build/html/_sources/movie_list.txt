电影列表获取接口
===================

获取电影列表
-------------------

::
  GET /movie/

请求参数说明

============= ======== ===============
name          type     value
============= ======== =============== 
city_id       int      查询目标城市id
============= ======== ===============

查询成功响应信息

::
  Status: 200 OK

::
  [
    [],
    {
    "nuomi_movie_id": "9724",
    "meituan_movie_id": "246063",
    "movie_name": "美人鱼",
    "taobao_movie_id": "151583"
    },
    {
    "nuomi_movie_id": "9746",
    "meituan_movie_id": "76365",
    "movie_name": "叶问3",
    "taobao_movie_id": "174519"
    },
    {
    "nuomi_movie_id": "9877",
    "meituan_movie_id": "334578",
    "movie_name": "圣斗士星矢",
    "taobao_movie_id": "89167"
    },
    {
    "nuomi_movie_id": "9808",
    "meituan_movie_id": "246051",
    "movie_name": "卧虎藏龙青冥宝剑",
    "taobao_movie_id": "145205"
    },
    {
    "nuomi_movie_id": "9744",
    "meituan_movie_id": "79202",
    "movie_name": "西游记之孙悟空三打白骨精",
    "taobao_movie_id": "151810"
    },
    {
    "nuomi_movie_id": "9876",
    "meituan_movie_id": "257392",
    "movie_name": "末日迷踪",
    "taobao_movie_id": "149109"
    },
    {
    "nuomi_movie_id": "9726",
    "meituan_movie_id": "248006",
    "movie_name": "澳门风云3",
    "taobao_movie_id": "180213"
    },
    {
    "nuomi_movie_id": "9871",
    "meituan_movie_id": "336868",
    "movie_name": "火影忍者剧场版博人传",
    "taobao_movie_id": "158974"
    },
    {
    "nuomi_movie_id": "9889",
    "meituan_movie_id": "246286",
    "movie_name": "疯狂动物城",
    "taobao_movie_id": "187271"
    },
    {
    "nuomi_movie_id": "9827",
    "meituan_movie_id": "342795",
    "movie_name": "高跟鞋先生",
    "taobao_movie_id": "185990"
    },
    {
    "nuomi_movie_id": "9723",
    "meituan_movie_id": "78535",
    "movie_name": "功夫熊猫3",
    "taobao_movie_id": "184389"
    },
    {
    "nuomi_movie_id": "9848",
    "meituan_movie_id": "344769",
    "movie_name": "诡娃",
    "taobao_movie_id": "186677"
    },
    {
    "nuomi_movie_id": "9887",
    "meituan_movie_id": "337020",
    "movie_name": "地心营救",
    "taobao_movie_id": "188072"
    },
    {
    "nuomi_movie_id": "9909",
    "meituan_movie_id": "246884",
    "movie_name": "谍影特工",
    "taobao_movie_id": "174860"
    },
    {
    "nuomi_movie_id": "9894",
    "meituan_movie_id": "345158",
    "movie_name": "托马斯和朋友们多多岛之迷失宝藏",
    "taobao_movie_id": "188025"
    },
    {
    "nuomi_movie_id": "9896",
    "meituan_movie_id": "345737",
    "movie_name": "夺命枪火",
    "taobao_movie_id": "188084"
    },
    {
    "nuomi_movie_id": "",
    "meituan_movie_id": "338412",
    "movie_name": "神战权力之眼",
    "taobao_movie_id": "151014"
    },
    {
    "nuomi_movie_id": "9832",
    "meituan_movie_id": "342783",
    "movie_name": "青蛙王国之冰冻大冒险",
    "taobao_movie_id": "186486"
    },
    {
    "nuomi_movie_id": "9890",
    "meituan_movie_id": "344495",
    "movie_name": "当我们年轻的时候",
    "taobao_movie_id": "188057"
    },
    {
    "nuomi_movie_id": "9854",
    "meituan_movie_id": "246301",
    "movie_name": "谋杀似水年华",
    "taobao_movie_id": "158147"
    },
    {
    "nuomi_movie_id": "9875",
    "meituan_movie_id": "345429",
    "movie_name": "致命怪谈",
    "taobao_movie_id": "187523"
    },
    {
    "nuomi_movie_id": "9550",
    "meituan_movie_id": "246509",
    "movie_name": "爱情麻辣烫之情定终身",
    "taobao_movie_id": "33682"
    },
    {
    "nuomi_movie_id": "9884",
    "meituan_movie_id": "345694",
    "movie_name": "恭喜发财之谈钱说爱",
    "taobao_movie_id": "187850"
    },
    {
    "nuomi_movie_id": "9910",
    "meituan_movie_id": "345787",
    "movie_name": "你是不是我的爱人",
    "taobao_movie_id": "188891"
    }

  ]

响应参数说明

================== ========== =============
name                type       value
================== ========== =============
movie_name          string    电影名
meituan_movie_id    string    美团电影ID
nuomi_movie_id      string    糯米电影ID
taobao_movie_id     string    淘宝电影ID
================== ========== =============

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




















