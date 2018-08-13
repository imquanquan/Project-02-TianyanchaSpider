# Project-02 TianyanSpider

use the selenium and Chrome tools implements crawl tianyan companie's data and store it into mongodb.																		
### Project Description

   通过给定的关键字爬取相关公司信息，本项目针对关键字 ‘测绘’、‘地理信息’等进行数据爬取，然后将数据存进 MongoDB。


### Environment
	
+ Python3.6.3
+ Selenium 3.8.0
+ Chromedriver V2.41
+ Chrome 版本 67.0.3396.99

chromedriver 镜像地址可查看 [npm.taobao.org](http://npm.taobao.org/mirrors/chromedriver/)
    
### Importance

   由于项目采用 selenium、Chrome，请注意 Chrome 与 Chromedriver 的版本匹配问题。天眼搜索查询普通用户仅支持 100 家，VIP用户支持 5000 家。详情页大部分信息则不受 VIP限制。

#### Hisory Version

+ 2018-08-13

	1、修改数据结构存储格式
	2、完善链接列表的获取
	3、将数据进行了轻微的清理
	4、调整爬取速度

+ 2018-08-07
  
  实现：公司基本信息包括，网址、注册时间、注册地点、法定代表人、经营范围、公司规模、公司专利、软件著作权、招标等信息
  
  缺点：爬虫速度过快、爬取数据量过大易引起天眼查的反爬策略，常见的为验证码问题以及账号登入问题。由于请求的数据多达2万条，总体爬虫效率较低，爬虫速度待改进。
 
  样例数据: 
           
    ![2018-08-07-data-example1](./images/2018-08-08_092058.png)
  
