---
title: markdown博客常用工具
tags: ['markdown', '博客']
key: 2022-12-31-markdown-boke-changyong-gongju.md
---

# 博客应用环境

github pages

jekyll-TeXt-theme

# 文章目录

_posts

# 文件名称

年-月-日-标题.MARKUP

2022-12-31-new-years-eve-is-awesome.md

# YAML头信息
```
---
title: markdown博客常用工具
tags: ['markdown', '博客']
key: 2022-12-31-markdown-boke-changyong-gongju.md
---
```

*配置key是为了页面展示评论功能*

# 帮助文档

[jekyll-TeXt-theme](https://kitian616.github.io/jekyll-TeXt-theme/docs/zh/quick-start) 参数配置、文章结构、页面布局

# 工具
## 在线代码运行
一个在线的前端代码编辑工具[codepen](https://codepen.io/)
代码在线运行工具[tool.lu](https://tool.lu/coderunner/)
## markdown工具
typora [帮助文档](https://support.typoraio.cn/zh/Markdown-Reference/) 破解 [1](https://www.ghxi.com/typora.html) [2](https://www.isharepc.com/32946.html) [3](https://foxirj.com/typora)

偏好设置-图像-上传服务器

picgo-core安装路径C:\Users\win_t\AppData\Roaming\Typora\picgo\win64

设置picgo.exe set uploader
picgo use uploader

# 图床

## 网址

1. 优秀
* 阿里云oss
* 腾讯云cos
2. 以下是听说优秀
* Vultr
* 般佤工
* 七牛云
* 又拍云
* UCloud
* Github
* SM.MS图床
* 路过图床
* Imgur 

## 工具

picgo [首页](https://picgo.github.io/PicGo-Doc/)

# 遇到的问题

## gitalk网络连接失败

gitalk构造函数中添加proxy参数，配置文件中指定proxy参数的值

我使用的代理网址是 `https://vercel.prohibitorum.top/github_access_token`

参考：

https://cuiqingcai.com/30010.html
https://prohibitorum.top/7cc2c97a15b4.html

