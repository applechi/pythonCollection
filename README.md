
# pythonCollection（python代码集合）

## json2mysql

这次更新了将一个json文件中的数据导入到mysql的脚本。 是用nodejs写的。

对应的文件是tomysql.js 有兴趣的同志可以研究下。


**本项目目前仅在python2.7下实验，其他版本暂不维护，请灵活使用**

- 文件下载器
- pdf合并工具
- 极客专栏文章下载
- 掘金小册下载
- 新浪微博爬虫

## 文件下载器（downloader.py）

>从数据库或者文件中读取文件url地址，并且下载到本地

依赖库：

- requests
- progressbar
- MySQLdb（如果不从数据库读取数据则不需要）


## pdf合并工具（pdfmerger.py）

>合并pdf文件

代码正在整理中..

## 极客专栏文章下载（geeksplider.py）

>将你购买的极客专栏，下载为json文件

**2019-5-30 更新**

近期geek网站加了一个限流的限制，以及请求时间戳的一些验证。

对应的python文件就没更新。加完代理池什么的应该就可以用了。

这次采用了一个新的套路：在浏览器控制台里执行js脚本，发送请求，再将数据存为json文件进行下载。

对应的js文件是geek.js  有兴趣的同学可以研究一下哈，个人感觉还是挺有意思的。



依赖库：

- requests

文件格式为：
```
{
    "article_title": "", 
    "audio_time": "", 
    "ctime": 1521993600, 
    "audio_size": 4375851, 
    "pid": 76, 
    "audio_url": "", 
    "mdhtml": "", 
    "audio_download_url": "", 
    "id": 4969, 
    "article_cover": ""
}
``` 

可以根据自己的需求灵活改动代码进行使用.

## 掘金小册下载（juejinxiaoce.py）

>将你购买的掘金小册，下载为json格式

依赖库：

- requests

文件格式为：

```
{
    "article_title": "", 
    "pid": "", 
    "mdhtml": "", 
    "mdtext": "", 
    "id": "", 
    "createdAt": ""
}
```

## 新浪微博爬虫（weibosplider.py）

>爬取某个人的新浪微博数据

依赖库：

- requests
- MySQLdb(如果不保存到数据库则不需要)
- logging

本脚本将数据直接存储到数据库，你也可以修改部分逻辑，存储到其他地方。

**灵活使用，代码仅供参考**

# issue

使用中遇到问题，可以在该项目下提issue [issues入口](https://github.com/maixiaojie/pythonCollection/issues)


# PR

如果你也有好用的小工具要分享，请new pull request
=======
# pythonCollection（python代码集合）

**如果对您有帮助的话，给个star哟~**

**本项目目前仅在python2.7下实验，其他版本暂不维护，请灵活使用**

- 文件下载器
- pdf合并工具
- 极客专栏文章下载
- 掘金小册下载
- 新浪微博爬虫

## 文件下载器（downloader.py）

>从数据库或者文件中读取文件url地址，并且下载到本地

依赖库：

- requests
- progressbar
- MySQLdb（如果不从数据库读取数据则不需要）


## pdf合并工具（pdfmerger.py）

>合并pdf文件

代码正在整理中..

## 极客专栏文章下载（geeksplider.py）

>将你购买的极客专栏，下载为json文件

依赖库：

- requests

文件格式为：
```
{
    "article_title": "", 
    "audio_time": "", 
    "ctime": 1521993600, 
    "audio_size": 4375851, 
    "pid": 76, 
    "audio_url": "", 
    "mdhtml": "", 
    "audio_download_url": "", 
    "id": 4969, 
    "article_cover": ""
}
``` 

可以根据自己的需求灵活改动代码进行使用.

## 掘金小册下载（juejinxiaoce.py）

>将你购买的掘金小册，下载为json格式

依赖库：

- requests

文件格式为：

```
{
    "article_title": "", 
    "pid": "", 
    "mdhtml": "", 
    "mdtext": "", 
    "id": "", 
    "createdAt": ""
}
```

## 新浪微博爬虫（weibosplider.py）

>爬取某个人的新浪微博数据

依赖库：

- requests
- MySQLdb(如果不保存到数据库则不需要)
- logging

本脚本将数据直接存储到数据库，你也可以修改部分逻辑，存储到其他地方。

**灵活使用，代码仅供参考**

# issue

使用中遇到问题，可以在该项目下提issue [issues入口](https://github.com/maixiaojie/pythonCollection/issues)


# PR

如果你也有好用的小工具要分享，请new pull request
>>>>>>> 9c2f63f36366393511dcb3d1adf2f02d675813ce
