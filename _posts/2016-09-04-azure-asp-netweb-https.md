---
id: 9853
title: 微软Azure ASP.Net/Web网站绑定域名、部署Https SSL加密证书教程
date: 2016-09-04T17:12:00+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=9853
permalink: /azure-asp-netweb-https.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "7480"
baidu_record:
  - "1"
bigfa_ding:
  - "1"
smilie_vote_3:
  - "1"
categories:
  - Asp.Net
  - Web开发
  - 未分类
---
上一篇《<a href="http://www.axiangblog.com/azure-asp-net-sql.html" target="_blank"  rel="nofollow" >微软Azure云服务体验一：快速搭建ASP.Net/Web应用+SQL、发布网站/数据库教程</a>》分享了网站搭建教程，这次笔者将为开发者、新老站长分享下如何在微软Azure云服务中为ASP.Net/Web网站绑定域名、部署Https SSL加密证书，让你的网站的地址栏加上一个小锁，更令人刮目相看。

<a href="http://www.axiangblog.com/azure-asp-netweb-https.html/azureweb-service7" rel="attachment wp-att-9860" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9860" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azureweb-service7.jpg" alt="azureweb-service7" width="450" height="293" /></a>

操作步骤：

1、登录国际版微软Azure仪表盘：<a href="https://portal.azure.com/" target="_blank"  rel="nofollow" >https://portal.azure.com/</a>

2、找到自己的对应的Web应用项目，进入《自定义域》，开始绑定顶级域名或二级域名，这里需要配合下第三方DNS解析服务商，例如DNSPod。

<a href="http://www.axiangblog.com/azure-asp-netweb-https.html/azureweb-service2" rel="attachment wp-att-9855" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9855" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azureweb-service2.jpg" alt="azureweb-service2" width="500" height="237" /></a>3、比如我们将wap.axiangblog.com二级域名绑定到微软Azure中，需要为该域名加至少2条记录，推荐A和TXT记录（或A和CName记录），为了避免冲突，首选A和TXT记录。

<a href="http://www.axiangblog.com/azure-asp-netweb-https.html/azureweb-service1" rel="attachment wp-att-9854" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9854" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azureweb-service1.jpg" alt="azureweb-service1" width="400" height="235" /></a>打开第三方DNSPod，https://www.dnspod.cn/，分别添加2条新记录：A记录填写微软Azure云服务器的IP地址，TXT记录填写Azure的二级域名，例如axiang.azurewebsites.net，保存生效。

4、回到微软Azure的《自定义域》，添加刚才的wap.axiangblog.com二级域名进行绑定，即可完成验证和添加任务。

<a href="http://www.axiangblog.com/azure-asp-netweb-https.html/azureweb-service3" rel="attachment wp-att-9856" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9856" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azureweb-service3.jpg" alt="azureweb-service3" width="300" height="335" /></a>5、接下来我们还需申请一个国内免费DV SSL证书，<a href="http://freessl.wosign.com/freessl" target="_blank"  rel="nofollow" >http://freessl.wosign.com/freessl</a>，自定义一个SSL私钥密钥，注：该证书支持不同服务器和环境的部署，例如Azure上使用了Windows Server IIS网络环境

<a href="http://www.axiangblog.com/azure-asp-netweb-https.html/azureweb-service5" rel="attachment wp-att-9858" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9858" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azureweb-service5.jpg" alt="azureweb-service5" width="450" height="338" /></a>6、同样回到微软Azure仪表盘，进入自己的项目，打开《SSL证书》，手动上载SSL证书和SSL私钥密钥，完成SSL绑定和验证。

<a href="http://www.axiangblog.com/azure-asp-netweb-https.html/azureweb-service6" rel="attachment wp-att-9859" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9859" src="http://www.axiangblog.com/wp-content/uploads/2016/09/azureweb-service6.jpg" alt="azureweb-service6" width="500" height="325" /></a>现在我们可以使用HTTPS加密协议访问自己的网站项目了，演示站：<a href="https://wap.axiangblog.com/" target="_blank"  rel="nofollow" >https://wap.axiangblog.com/</a>

相关教程：

《<a href="http://www.axiangblog.com/azure-asp-net-sql.html" target="_blank"  rel="nofollow" >微软Azure快速搭建ASP.Net/Web应用+SQL、发布网站/数据库教程</a>》

《<a href="http://www.axiangblog.com/ms-azure-for-dreamspark-test.html" target="_blank" rel="nofollow" >微软免费版Azure for DreamSpark搭建Web Apps/HTML5网站教程 云就是强大</a>》

《<a href="http://www.axiangblog.com/windows-azure-php-mysql.html" target="_blank" rel="nofollow" >Windows Azure免费空间如何搭建PHP网站/数据库、域名绑定</a>》

《<a href="http://www.axiangblog.com/windows-azure-website-virtual-machine.html" target="_blank" rel="nofollow" >中国版Windows Azure免费空间如何建站、自定义远程虚拟机？</a>》

<a href="http://www.axiangblog.com/windows-azure-ebook.html" target="_blank" rel="nofollow" >《Windows Azure介绍》简体中文版电子书下载</a>