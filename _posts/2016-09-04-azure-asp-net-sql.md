---
id: 9836
title: 微软Azure快速搭建ASP.Net/Web应用+SQL、发布网站/数据库教程
date: 2016-09-04T16:07:36+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=9836
permalink: /azure-asp-net-sql.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "5467"
baidu_record:
  - "1"
smilie_vote_1:
  - "1"
categories:
  - Asp.Net
  - Web开发
  - 未分类
---
微软开发者项目权益“Developer Program Benefit”在今年上半年就向全球开发者开放，尤其赠送了一年Azure云服务福利，其中就包括各类微软Azure云服务中的基础和高级服务，不容错过。这次笔者将带大家一起熟悉下快速搭建ASP.Net/Web+SQL数据库、发布网站的操作。

准备工作：<a href="https://myprodscussu1.app.vssubscriptions.visualstudio.com/" target="_blank"  rel="nofollow" >注册Visual Studio Dev Essentials订阅服务</a>、<a href="https://azure.microsoft.com/zh-cn/offers/ms-azr-0022p/" target="_blank"  rel="nofollow" >领取“Developer Program Benefit”Azure云服务</a>

微软Azure云服务是一个综合性的服务器，玩家可以在商店中一键式部署各类Web应用或SQL数据库，也可以启用第三方的扩展等服务，目前Web项目支持 .NET、PHP、Node.js、HTML5或Python开发站点。

<a href="http://www.axiangblog.com/azure-asp-net-sql.html/azure-web-sql1" rel="attachment wp-att-9838" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9838" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azure-web-sql1.jpg" alt="azure-web-sql1" width="500" height="330" /></a>操作步骤：

1、登录国际版微软Azure仪表盘：<a href="https://portal.azure.com/" target="_blank"  rel="nofollow" >https://portal.azure.com/</a>

2、新建项目，从应用商店中找到《Web应用+SQL》项目搭建，填写Web应用名称，默认使用了二级网址的访问方式，例如<a href="http://axiang.azurewebsites.net/" target="_blank"  rel="nofollow" >http://axiang.azurewebsites.net/</a>

<a href="http://www.axiangblog.com/azure-asp-net-sql.html/azure-web-sql2" rel="attachment wp-att-9839" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9839" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azure-web-sql2.jpg" alt="azure-web-sql2" width="500" height="389" /></a>3、每个Web应用都需要一个APP Services计划/资源组，新建一个即可，可手动选择Azure全球服务器中位置、规格以及定价，日常测试可以选择一个S1标准或B1标准模式。

<a href="http://www.axiangblog.com/azure-asp-net-sql.html/azure-web-sql3" rel="attachment wp-att-9840" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9840" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azure-web-sql3.jpg" alt="azure-web-sql3" width="500" height="274" /></a>4、选择之后，继续配置SQL数据库，依次填写数据库名称，数据库的配置，差不多一个B基本计划足够了、新建一个目标服务器，默认采用了二级网址访问，例如“服务器名称.database.windows.net”。

<a href="http://www.axiangblog.com/azure-asp-net-sql.html/azure-web-sql4" rel="attachment wp-att-9841" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9841" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azure-web-sql4.jpg" alt="azure-web-sql4" width="500" height="309" /></a>5、搭建完数据库后，别忘了配置SQL管理员的用户名和密码，默认需要大小写字母、数字以及字符组成；

<a href="http://www.axiangblog.com/azure-asp-net-sql.html/azure-web-sql5" rel="attachment wp-att-9842" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9842" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azure-web-sql5.jpg" alt="azure-web-sql5" width="400" height="324" /></a>6、到这里基本上，我们的《ASP.Net/Web应用+SQL数据库》项目基本搞定，整个队列都隶属于Azure资源组。

<a href="http://www.axiangblog.com/azure-asp-net-sql.html/azure-web-sql6" rel="attachment wp-att-9843" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9843" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azure-web-sql6.jpg" alt="azure-web-sql6" width="500" height="354" /></a>7、现在，我们可以在Visual Studio 2015开发工具，创建一个Asp.NET Web项目，然后右击项目，直接“发布Web”到微软Azure的App Services资源组中，即可发布网站。

<a href="http://www.axiangblog.com/azure-asp-net-sql.html/azure-web-sql7" rel="attachment wp-att-9847" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9847" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azure-web-sql7.jpg" alt="azure-web-sql7" width="500" height="342" /></a>8、当然动态网站离不开SQL数据库，不过微软Azure SQL默认绑定了用户的客户端IP，无法直接访问。

<a href="http://www.axiangblog.com/azure-asp-net-sql.html/azure-web-sql8" rel="attachment wp-att-9845" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9845" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azure-web-sql8.jpg" alt="azure-web-sql8" width="500" height="283" /></a>因此，需要在微软Azure SQL数据库打开《防火墙设置》，允许客户端访问Azure服务，手动添加客户端IP地址，最后保存完成生效。

<a href="http://www.axiangblog.com/azure-asp-net-sql.html/azure-web-sql9" rel="attachment wp-att-9846" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9846" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azure-web-sql9.jpg" alt="azure-web-sql9" width="450" height="419" /></a>最后，我们可以使用SQL Server Management Studio本地数据库管理工具连接Azure SQL，完成数据库表的创建以及SQL语句的查询和导入等任务。

相关教程：

《<a href="http://www.axiangblog.com/ms-azure-for-dreamspark-test.html" target="_blank" rel="nofollow" >微软免费版Azure for DreamSpark搭建Web Apps/HTML5网站教程 云就是强大</a>》

《<a href="http://www.axiangblog.com/windows-azure-php-mysql.html" target="_blank" rel="nofollow" >Windows Azure免费空间如何搭建PHP网站/数据库、域名绑定</a>》

《<a href="http://www.axiangblog.com/windows-azure-website-virtual-machine.html" target="_blank" rel="nofollow" >中国版Windows Azure免费空间如何建站、自定义远程虚拟机？</a>》

<a href="http://www.axiangblog.com/windows-azure-ebook.html" target="_blank" rel="nofollow" >《Windows Azure介绍》简体中文版电子书下载</a>