## 1 运行环境和python库

### 先说下运行环境：

- python3.5
- python库

### 主要涉及以下一些python库：

- requests
- BeautifulSoup
- multiprocessing
- pymongo
- itertools

## 2 爬取的主要步骤

- 根据关键字、城市、以及页面编号生成需要爬取的网页链接
- 用requests获取相应的网页内容
- 用BeautifulSoup解析，获取需要的关键信息
- 将爬取的信息存入MongoDB数据库中，插入新记录或更新已有记录
- 用multiprocessing启动多进程进行爬取，提高运行效率

## 3 文件组成

- 信息配置文件“config.py”
- 爬虫主运行文件“spider.py”
- 在配置文件中设置需要爬取的信息，然后运行主程序进行内容抓取。