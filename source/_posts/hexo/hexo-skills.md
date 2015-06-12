title: "Hexo生成sitemap站点地图的方法"
date: 2015-06-10 00:00:00
categories: hexo
tags: [hexo,sitemap,站点地图]
---
1、安装插件：
```
npm install hexo-generator-sitemap --save
npm install hexo-generator-baidu-sitemap --save
```

2、在博客目录的_config.yml中添加如下代码：
```
# 自动生成sitemap
sitemap:
path: sitemap.xml
baidusitemap:
path: baidusitemap.xml
```

3、hexo编译的时候会自动在根目录生成站点地图