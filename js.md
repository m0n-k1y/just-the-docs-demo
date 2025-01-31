---
title: 微信小程序
layout: home
---

# 初识微信小程序



## 小程序的简单介绍

小程序是在 2017 年 1 月 9 号正式上线的。

小程序最大的特点是不需要下载安装，“用完即走”。

在最早期的时候，小程序的诞生没有造成行业的冲击，之后，在 2017 年年底的时候，出现了一个叫做跳一跳的游戏

![image-20230110154916910](https://xiejie-typora.oss-cn-chengdu.aliyuncs.com/2023-01-10-074917.png)

小程序目前一般就应用在一些轻量级别的应用上面，用户没有必要下载，直接通过小程序操作，用完即走。

- 工具类：嘀嘀打车、美团、打卡
- 资讯类：网易新闻、豆瓣
- 电商：京东、网易严选、拼多多
- 小型游戏：斗地主、头脑风暴

但是重型的应用就不适合用小程序来做了，王者荣耀、绝地求生..



## 小程序的准备工作

- [小程序开发指南](https://developers.weixin.qq.com/ebook?action=get_post_info&docid=0008aeea9a8978ab0086a685851c0a)
- [微信开放文档](https://developers.weixin.qq.com/miniprogram/dev/framework/)



首先需要申请一个账号，注意注册的邮箱不要是之前用过的，最好专门拿一个新的邮箱来进行申请。

申请完账号之后，有一个非常重要的东西，叫做 AppID

<img src="https://xiejie-typora.oss-cn-chengdu.aliyuncs.com/2023-01-10-075732.png" alt="image-20230110155732169" style="zoom:50%;" />

进入之后，在【开发】-【开发管理】-【开发设置】下面能够找到自己的 AppID，这个 ID 非常重要，每次我们创建项目的时候，都需要填写这个 ID

![image-20230110155940956](https://xiejie-typora.oss-cn-chengdu.aliyuncs.com/2023-01-10-075941.png)



接下来是安装“微信开发者工具”，前往官网提供的地址，选择操作系统对应的版本，下载安装即可。

![image-20230110160705177](https://xiejie-typora.oss-cn-chengdu.aliyuncs.com/2023-01-10-080705.png)



## 初始化一个小程序的项目

初始化好一个项目之后，整体的初始目录如下：

- pages：小程序里面目前所有的页面
  - pages 里面一个文件夹表示一个页面，展开之后又分为 4 个部分
  - js：该页面对应的逻辑
  - json：该页面的一些配置信息
  - wxml：全称叫做 wei xin markup language，基本上语法就和 html 一样的，只不过不能使用 html 里面的那些标签，使用的是小程序为我们提供的组件，view、text
  - wxss：全称叫做 wei xin style sheets，负责样式的，基本上就和 css 是一样的
- utils：工具目录
- .eslintrc.js：eslint 配置文件
- app.js：项目的入口 JS 文件
- app.json：全局的配置文件，可以配置 tabBar、navigation 等
- app.wxsss：全局的 CSS 样式

----