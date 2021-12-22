---
id: 8574
title: 解决301重定向、分类目录失效等 阿里云主机WordPress网站常见问题方案
date: 2015-12-16T22:52:26+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=8574
permalink: /aliyun-wordpress-fix.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
baidu_record:
  - "1"
views:
  - "4217"
smilie_vote_2:
  - "1"
categories:
  - Web开发
  - 未分类
---
不久前，笔者将博客搬到了免费版阿里云主机平台，整个搬家过程也是非常顺利，上手熟悉，尤其是刚刚更新到Wordpress 4.4新版，响应还是很及时。刚搬家后，笔者也发现了阿里云搭建Wordpress网站一些日常使用问题，顺便整理下相关解决方案，一起来学习下。

访问阿里云控制台：<a href="http://home.console.aliyun.com/" target="_blank" rel="nofollow" >http://home.console.aliyun.com/</a>

<!--more-->

  
1、登陆WordPress提示错误：Cookies被阻止或者您的浏览器不支持&#8230;

<a href="http://www.axiangblog.com/aliyun-wordpress-fix.html/wordpress-aliyun5" rel="attachment wp-att-8578" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8578" src="http://www.axiangblog.com/wp-content/uploads/2015/12/wordpress-aliyun5.jpg" alt="wordpress-aliyun5" width="360" height="277" /></a>  
官方方案：访问阿里云后台，选中“高级环境设置”，设置php.ini，将其中的“输出缓冲区数据块”设置开启，即可。

<a href="http://www.axiangblog.com/aliyun-wordpress-fix.html/wordpress-aliyun2" rel="attachment wp-att-8576" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8576" src="http://www.axiangblog.com/wp-content/uploads/2015/12/wordpress-aliyun2.jpg" alt="wordpress-aliyun2" width="500" height="340" /></a>  
2、域名301重定向www.域名

笔者方案：访问阿里云后台，选中“基本环境设置”，设置301定向，添加所需的域名和重定向域名，即可。

<a href="http://www.axiangblog.com/aliyun-wordpress-fix.html/wordpress-aliyun1" rel="attachment wp-att-8575" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8575" src="http://www.axiangblog.com/wp-content/uploads/2015/12/wordpress-aliyun1.jpg" alt="wordpress-aliyun1" width="500" height="215" /></a>  
3、Wordpress分类目录丢失、标签丢失或失效

网上方案：进入wordpress后台》设置》固定链接，先选择其他任意链接样式，按保存；然后再恢复成%postname%.html等设置。

<a href="http://www.axiangblog.com/aliyun-wordpress-fix.html/wordpress-aliyun3" rel="attachment wp-att-8577" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8577" src="http://www.axiangblog.com/wp-content/uploads/2015/12/wordpress-aliyun3.jpg" alt="wordpress-aliyun3" width="500" height="198" /></a>  
笔者方案：进入阿里云PHPAdmin后台，选中所有数据库表，依次优化和修复，即可解决。

相关教程：《<a href="http://www.axiangblog.com/aliyun-vps-settting.html" target="_blank" rel="nofollow" >阿里云绑定域名、FTP上传、数据库导入、Worpress博客搬家/备份教程</a>》