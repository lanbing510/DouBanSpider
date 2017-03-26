## 豆瓣读书爬虫

Python所写，豆瓣读书的爬虫，方便大家搜罗各种美美书！


### 更新

最近爬下了豆瓣所有的图书信息（3088633本，2138386KB），并做了一个界面方面与数据库交互来搜罗好书。 注：这里的代码不是爬下所有书籍所用的代码，仅供参考。有机会的时候再公开代码和爬下的所有数据。


交互界面截图示例：

![Aaron Swartz](https://github.com/lanbing510/DouBanSpider/raw/master/screenshots/sobook.jpg)

查询结果截图示例：

![Aaron Swartz](https://github.com/lanbing510/DouBanSpider/raw/master/screenshots/result.jpg)


### 更新

最近爬书发现豆瓣的页面规则发生了变化，导致不能爬到评价人数，由此对代码进行了相应的更新，并爬了一些新的数据(并不全)。



### 实现功能

1 可以爬下豆瓣读书标签下的所有图书 

2 按评分排名依次存储

3 存储到Excel中，可方便大家筛选搜罗，比如筛选评价人数>1000的高分书籍；可依据不同的主题存储到Excel不同的Sheet 

4 采用User Agent伪装为浏览器进行爬取，并加入随机延时来更好的模仿浏览器行为，避免爬虫被封（更新于 2015-5-20）

### 效果截图

试着小小运行了下，爬了七八万本书，结果在book_list.xlsx中，截图如下：

![Aaron Swartz](https://github.com/lanbing510/DouBanSpider/raw/master/screenshots/douban.jpg)


代码刚写一小时，更多功能有待增加


声明：受@plough同学启发，再其代码基础上进行的创作，感谢@plough




