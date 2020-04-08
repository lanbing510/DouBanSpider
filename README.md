## 豆瓣读书爬虫

Python所写，豆瓣读书的爬虫，方便大家搜罗各种美美书！

### 更新

今年年初又爬了一遍豆瓣图书数据，爬下了3000000+条目，这次爬的时候特意爬取了每个图书页面中的“喜欢读XX的人也喜欢条目XX”，最近对数据进行了处理和可视化做了这个新的WebApp（随意取名书海星空），WebApp的截图如下。

![Aaron Swartz](https://github.com/lanbing510/DouBanSpider/raw/master/screenshots/shxk.png)

![Aaron Swartz](https://github.com/lanbing510/DouBanSpider/raw/master/screenshots/shxk1.png)

书海星空WebApp中每本书作为一个节点包含评价人数、评分、被链接数（类似Google的RankPage算法根据网页被链接的数目来排网页的重要性，一般越好的书籍被链接的数目也越多）、链入的图书节点、链出的图书节点等信息。作为[好书一下](http://sobook.lanbing510.info)的补充（为了找经典好书读之前做了[好书一下](http://sobook.lanbing510.info)：自己可通过评价人数、评分等筛选寻找好书），书海星空可以根据看过的或找到的好书顺藤摸瓜来找相关的更多经典好书，书海中尽情泛舟，找到自己喜欢的宝藏。我平时可以里面泡上一整天。

想获取书海星空源码及数据，移步到这里：[书海星空](https://zhuanlan.zhihu.com/p/123271223)。


### 更新

#### 写在前面

通过豆瓣评分和评价人数等规则，可非常好的探索挖掘经典图书和隐藏好书，从中更高效地汲取书中智慧。鉴于此，在16年的时候爬下了豆瓣所有的读书数据并做了个简单的WebApp接口方便自己挖掘查找和阅读好书。一直在用自己搞的这个搜书工具，觉得特别好，最近就再次爬了一遍豆瓣读书的数据，总共更新了3232088本图书信息。最近想把这个工具分享给大家，就自掏腰包租了一年的阿里云服务器，将WebApp放了上去，喜欢读书和不断学习的朋友可以访问[好书一下](http://sobook.lanbing510.info)使用(推荐使用电脑访问)。


#### 使用说明

好书一下的首页如下。输入你所想查找相关书的关键字、评价分数高于的数值（一般高于8分就是不错的书，高于9分就是很好的书）、评价人数多于的数值（评价分数又高、人数又多的往往是经典之作），选定排序方法，点击好书一下就可以查找好书啦！

![Aaron Swartz](https://github.com/lanbing510/DouBanSpider/raw/master/screenshots/sobook1.png)

查找结果截图示例如下。

![Aaron Swartz](https://github.com/lanbing510/DouBanSpider/raw/master/screenshots/sobook2.jpg)

最后希望该工具能对你有所帮助，让你在挑选好书不断学习的路上走的更远！

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




