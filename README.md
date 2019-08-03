妹子图（mzitu.com）全站图片爬取，增量更新。  
图片按照专辑保存，保留了专辑与标签的关联关系。
- `asyncio`
- `aiohttp`
- `SQLAlchemy`
- `sqlite`    

主要特点：使用官方的`asyncio`库和第三方`aiohttp`进行异步爬取，可以自定义协程数量来控制爬取速度，
在不影响网站正常运行的前提下学习Python的异步编程。

**使用：**  
在命令行下，切换到文件目录，  
首先根据`requirements.txt`配置环境：
` pip install -r requirements.txt`  
然后执行
`python main.py "D:/mzitu"`     

由于没有配置代理IP等反爬措施，爬取速度设置的比较慢，网页爬取
默认开启一个协程，下载图片默认开启8个协程，
一般1-2h就可以完成。之后运行会自动比对数据库数据和网站数据，进行增量更新。
> 实际使用时请改为自己的路径   

> 声明：仅供学习交流，请勿对网站正常运行造成影响。


