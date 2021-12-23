---
id: 5293
title: 中国版Windows Azure免费空间如何建站、自定义远程虚拟机？
date: 2014-07-16T14:23:56+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=5293
permalink: /windows-azure-website-virtual-machine.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "11946"
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:5297;s:11:"_thumb_type";s:10:"attachment";}'
categories:
  - Asp.Net
  - Web开发
  - 未分类
---
近期，阿象分享了<a href="http://www.axiangblog.com/azure-free.html" target="_blank" rel="nofollow" >限时免费领取中国版Windows Azure试用账户</a>，相信各位码农、开发者、站长，已成功申请注册中国版Azure，简单体验了微软公有云的魅力。当然，阿象也在Windows Azure平台上成功创建第一个测试网站、第一台远程超级虚拟机（四核心、28G物理内存），非常便于以后的学习、测试和开发工作。

下面，阿象也简单分享了如何在中国版Windows Azure免费空间搭建网站、自定义虚拟机，具体参考如下：

**一、建站篇  
** 

1、访问中国版Windows Azure后台：<a href="https://manage.windowsazure.cn/" target="_blank"  rel="nofollow" >https://manage.windowsazure.cn/</a> ，输入之前的团体账户和密码，登录

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur1.jpg) 

目前，中国版Windows Azure平台已支持网站（HTML/PHP/ASP.Net等）、虚拟机（支持创建Windows Server、Ubuntu平台）、SQL数据库、云存储、虚拟网络等服务；

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur2.jpg) 

2、点击底部的**新建**，选择网站，即可快速新建一个空白站点，支持设置二级域名、自定义网站地区（可选中国北部、东部），最后**创建**，即可生效；

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur3.jpg) 

3、当新建新站点后，我们还需要手动创建新站点的远程FTP访问入口、FTP账户密码，这时选中当前的**空白站点**，打开**仪表盘**，点击&#8221;速览&#8221;栏目下的&#8221;**重置部署凭据**&#8220;；

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur4.jpg) 

4、分别输入用户名、密码，完成账户创建工作；

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur5.jpg) 

5、接着访问仪表盘，点击右侧的&#8221;**FTP主机名**&#8220;，该名称也是FTP远程访问路径，依次输入&#8221;**二级域名+\+用户名**&#8220;格式的用户名和密码，注意用\分开；

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur6.jpg) 

6、最后，我们成功登陆新站点的FTP远程服务器，具体网站程序路径为**/site/wwwroot/**；

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur7.jpg) 

7、当然，我们也可以用FTP客户端软件，手动上传、下载、编辑网站数据，即可完成网站搭建工作。

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur8.jpg) 

**二、虚拟机篇  
** 

除了支持创建网站外，中国版Windows Azure也为开发者朋友提供远程虚拟机服务，其中免费账户允许体验原生四核CPU、28G内存的虚拟机，真正感受下公有云的强大之处。

1、同样**新建**，选择**虚拟机**，输入**二级域名、系统平台**（可选Windows Server 2012 R2/2012英语版和中文版、Ubuntu、SUSE Linux）**、硬件配置**（可选处理器核心、物理内存）**、系统账户+密码**、以及虚拟机的**地理区域**，最后选择创建；

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur9.jpg) 

2、当完成虚拟机创建后，点击底部的**连接**，即可手动下载一个RDP专用**远程桌面连接**快捷方式；

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur10.jpg) 

3、双击运行该**远程桌面连接**，输入系统账户+密码，即可直接登陆远程虚拟机，如下图所示；

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur11.jpg) 

本次测试中，阿象手动搭建了一个Server 2012 R2数据中心版本，四核心Xeon处理器，28G物理内存，整体性能非常强悍，非常便于创建VS 2013编译环境。

![](http://www.axiangblog.com/wp-content/uploads/2014/07/071614_1423_WindowsAzur12.jpg) 

<a href="http://www.axiangblog.com/wp-content/uploads/2014/07/azure13.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5297" src="http://www.axiangblog.com/wp-content/uploads/2014/07/azure13.jpg" alt="azure13" width="563" height="355" /></a>

阿象推荐：《Windows Azure介绍》中文电子书免费下载：5.5MB

<a href="http://download.microsoft.com/download/7/E/0/7E0897FF-513B-4C69-A416-60F7DFB99BFB/Ebook%20Windows%20Azure%20Introductionfor%20IT%20Pro.pdf" target="_blank"  rel="nofollow" >http://download.microsoft.com/download/7/E/0/7E0897FF-513B-4C69-A416-60F7DFB99BFB/Ebook%20Windows%20Azure%20Introductionfor%20IT%20Pro.pdf</a>