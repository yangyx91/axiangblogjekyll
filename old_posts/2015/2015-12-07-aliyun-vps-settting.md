---
id: 8390
title: 阿里云绑定域名、FTP上传、数据库导入、Worpress博客搬家/备份教程
date: 2015-12-07T09:49:49+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=8390
permalink: /aliyun-vps-settting.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "3932"
baidu_record:
  - "1"
categories:
  - Asp.Net
  - Web开发
  - Win10
  - 未分类
---
上周末，笔者因海外主机维护忙着对博客搬家，挑来跳去，最终还是选择了阿里云（免费版），可选国内青岛机房，默认配置1G空间、10G/月流量和50M数据库，基本满足了博客日常需求，值得一试，下面笔者简单分享下阿里云主机的相关操作教程：

<a href="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun01.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8391" src="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun01.jpg" alt="aliyun01" width="500" height="311" /></a><!--more-->

  
1、领取免费2年版阿里云主机，<a href="http://wanwang.aliyun.com/promotion/free-times/" target="_blank" rel="nofollow" >http://wanwang.aliyun.com/promotion/free-times/</a>

2、领取成功后，即可访问主机后台（控制台），<a href="http://netcn.console.aliyun.com/core/host/list2" target="_blank" rel="nofollow" >点击这里</a>，在这里罗列了主机基本信息，包括IP、临时域名（可绑定20个域名），管理入口等内容。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun03.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8393" src="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun03.jpg" alt="aliyun03" width="500" height="202" /></a>  
3、选中主机基本信息》绑定域名，即可手动添加多个域名，同时也能使用阿里云代备案服务，效率不错。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun02.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8392" src="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun02.jpg" alt="aliyun02" width="500" height="454" /></a>  
4、选中管理进入主机信息（初次使用主机需初始化，最高可选PHP5.5+MYSQL 5.1配置，支持HTML5环境），完成初始化后即可获取到FTP登录名、数据库用户名、数据库名称、设置登录密码。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun04.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8394" src="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun04.jpg" alt="aliyun04" width="500" height="280" /></a>  
一般FTP名称为：你的FTP登录名.my3w.com，使用FTP上传工具即可把自己网站程序、论坛、WP博客压缩包上传，然后使用主机自带的“文件解压缩”（linux支持zip和tar，windows支持zip和rar）解压到根目录，即可访问。

5、修改Wordpress博客配置文件wp-config.php，重新适配新的阿里云服务器；

**/*\* WordPress 数据库的名称 \*/**  
**define(&#8216;DB\_NAME&#8217;, &#8216;XXXXXXX396\_db&#8217;);**

**/*\* MySQL 数据库用户名 \*/**  
**define(&#8216;DB_USER&#8217;, &#8216;XXXXXXX396&#8217;);**

**/*\* MySQL 数据库密码 \*/**  
**define(&#8216;DB_PASSWORD&#8217;, &#8216;你设置的密码XXX&#8217;);**

**/*\* MySQL 主机 \*/**  
**define(&#8216;DB_HOST&#8217;, &#8216;XXXXXXX396.my3w.com&#8217;);**

6、导入数据库只需借助阿里云的phpmyadmin面板，<a href="http://phpmyadmin.hichina.com/phpmyadmin/index.php" target="_blank" rel="nofollow" >点击这里</a>，登录后选择导入，手动导入原先网站的SQL数据。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun06.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8396" src="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun06.jpg" alt="aliyun06" width="488" height="217" /></a>  
小贴士：《**虚拟主机导入MYSQL数据报错：unknown collation：utf8mb4\_unicode\_ci**》

问题原因：目前，虚拟主机配备的MYSQL数据库版本是5.1.48，不支持utf8mb4字符集，需要MySQL 5.5以上才支持

解决方法：使用记事本手动打开.sql文件，通过ctrl+h将该文件的中的CHARSET = utf8mb4全部替换成CHARSET = utf8，将COLLATE = utf8mb4\_unicode\_ci 全部替换为COLLATE = utf8\_general\_ci，然后重新导入测试，修改之前建议先对源文件做备份。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun05.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8395" src="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun05.jpg" alt="aliyun05" width="500" height="229" /></a>  
7、一切配置完成后，现在访问主页，即可正常使用网站了，ping值也很低，博客整体体验极大改善。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun07.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8397" src="http://www.axiangblog.com/wp-content/uploads/2015/12/aliyun07.jpg" alt="aliyun07" width="450" height="198" /></a>  
备注：阿里云主机也支持网站数据库备份、网站搬家以及文件压缩服务，读者们可以自行测试。