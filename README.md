# 跟着轮子哥有肉吃

此爬虫程序的唯一作用为：根据关键词定向下载轮子哥赞过的回答里面的的素（mei）材（nv）图片。

## 服用说明

### 原理
定向抓取轮子哥（理论上你也可以在zhihuclient.py里面修改目标用户）赞过的所有带图片回答，然后按照预设的关键词筛选出目标图片，并保存到本地。

### 环境与依赖

* 本程序运行的python版本 >= Python 3.5
* aiohttp,；
* BeautifulSoup

### how to start

- 当前目录下新建 auth.py，按如下格式写入你的知乎账号。默认会优先使用邮箱登陆。

    email = 'xxx@xxx.xxx'
    phone_num = 'xxxxxxxxxxx'
    password = 'xxxxx'

- 在 config.py 中可以对爬取页面的速度作调整，建议间隔放宽一点避免触发知乎的反爬虫机制

- 在 keywords.py 中可以修改爬取的关键字。

- 然后运行

    python3 main.py
    
- 图片会自动存放在 img 目录下，此时请打开服用
