使用django框架
==== 
#web_search模拟fofa做的搜索引擎--
----
        在setting.py下 DATABASES 配置数据库创建http_information数据库
        CREATE TABLE httpdata (id BIGINT(7) NOT NULL AUTO_INCREMENT, ip VARCHAR(200),title VARCHAR(10000),header VARCHAR(10000), created TIMESTAMP DEFAULT CURRENT_TIMESTAMP, PRIMARY KEY(id));创建表

![](https://github.com/cuijianxiong/web_search/blob/master/1.png) 
![](https://github.com/cuijianxiong/web_search/blob/master/2.png) 



    http://127.0.0.1/webshell/  为web指纹识别集成了大量fofa规则
    http://127.0.0.1/search/ 为web搜索
    hostscan下hostscan.py搜索web指纹并录入数据库中
    未完成:web指纹和web搜索结合
# 2017.03.26
----
更新了查询分页显示  修改了data数据库  用于django自带生成方法
