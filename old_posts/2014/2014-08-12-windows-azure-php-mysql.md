---
id: 5661
title: Windows Azure免费空间如何搭建PHP网站/数据库、域名绑定
date: 2014-08-12T23:54:12+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=5661
permalink: /windows-azure-php-mysql.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "18176"
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:5660;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_2:
  - "1"
categories:
  - Asp.Net
  - Web开发
  - 未分类
---
7月份，阿象为大伙介绍了<a href="http://www.axiangblog.com/windows-azure-website-virtual-machine.html" target="_blank"  rel="nofollow" >中国版Windows Azure如何建站、自定义远程虚拟机</a>，最高可选四核、28G内存的服务器，相信不少站长、开发者用户大呼过瘾。不过Azure建站系统仅支持SQL数据库，并不支持大家熟悉的MySQL平台。

那如何搭建PHP网站，日常中的WordPress博客、PHPWind/Discuz！等论坛程序都需要完整的PHP+MySQL平台环境，这时我们可以直接利用Azure平台的Windows Server 2012 R2云系统，借助IIS 8.5+PHP+MySQL三大件，即可搭建一个完整的PHP网站，而且支持绑定顶级域名，可以外网访问。

**阿象点评**：整个操作好比本地搭建IIS+PHP环境，具体可以参考《<a href="http://www.axiangblog.com/win8-1-iis8-5php5-5-4.html" target="_blank"  rel="nofollow" >Win8.1系统下配置搭建IIS8.5+PHP5.5.4</a>》，同时阿象还将补充下MySQL、域名绑定等内容。

**准备工作：  
** 

一、PHP 5.5.X，根据系统版本下载32位/64位，官网：<a href="http://windows.php.net/download" target="_blank"  rel="nofollow" >http://windows.php.net/download</a>

二、PHPMyAdmin数据库管理工具，官网：<a href="http://www.phpmyadmin.net/" target="_blank"  rel="nofollow" >http://www.phpmyadmin.net/</a>

三、MySQL数据库工具，访问官网：<a href="http://dev.mysql.com/downloads/mysql/" target="_blank"  rel="nofollow" >http://dev.mysql.com/downloads/mysql/</a>

四、PHP程序任一，例如PHPWind程序

**操作步骤：  
** 

**一、创建Azure虚拟机**（以Windows server 2012 r2为例）

1、访问中国版Azure后台：<a href="https://manage.windowsazure.cn/" target="_blank"  rel="nofollow" >https://manage.windowsazure.cn/</a> ，选择**新建虚拟机**，最高可选四核心、28G内存，设置虚拟机用户名和密码；

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur1.jpg) 

2、稍等片刻，完成虚拟机创建后，选中刚才创建的**虚拟机**，打开**端口**，手动添加HTTP名称和80端口（必选）；

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur2.jpg) 

3、稍等片刻，即可开启HTTP端口服务；

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur3.jpg) 

4、最后，点击底部的**连接**，即可手动下载一个RDP专用远程桌面连接快捷方式，双击运行该远程桌面连接，输入系统账户+密码，即可直接登陆远程虚拟机。

&nbsp;

**二、搭建IIS+PHP环境  
** 

1、远程登陆Windows Server 2012 R2虚拟机，打开服务器管理器，选择添加和功能向导，手动勾选&#8221;Web服务器（IIS）&#8221;，如下图所示。

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur4.jpg) 

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur5.jpg) 

2、在角色服务中，**必选CGI**应用程序开发，如下图；

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur6.jpg)![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur7.jpg) 

3、完成IIS功能和角色添加后，即可用IE访问<a href="http://127.0.0.1" target="_blank"  rel="nofollow" >http://127.0.0.1</a> ，检查能否打开IIS 8.5多国语言欢迎界面

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur8.jpg) 

4、下载PHP程序包，例如下载VC11 x64 Thread Safe 版本的压缩包，并解压到**C:\inetpub\php**目录;

5、打开**服务器管理器**，选择管理，进入**Internet信息服务(IIS)管理器**，选中当前的网站，双击IIS功能区中&#8221;**处理程序映射**&#8220;；

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur9.jpg) 

6、**选择添加模块映射**，请求路径输入&#8221;***.php**&#8220;，模块选择**FastCgiModule**模式，可执行文件时，文件格式可以选择exe程序和选择路径：**C:\inetpub\php\php-cgi.exe**，名称比如php，最后确定添加模块映射。

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur10.jpg) 

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur11.jpg) 

7、手动给网站添加默认文档：**default.php**和**index.php**两个文档；

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur12.jpg) 

8、配置PHP：进入**C:\inetpub\php**目录，重命名文件php.ini-development改名为php.ini；

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur13.jpg) 

9、用记事本打开编辑php.ini文件，阿象建议用Ctrl+F搜索定位，将PHP环境默认的date.timezone修改为date.timezone=&#8221;Asia/Hongkong&#8221;，即修改当前的系统时区, 同时将前面的分号&#8221;;&#8221;删除，即可生效。

&nbsp;

除此之外，我们还得激活PHP相关扩展、设置PHP扩展目录，即将相应dll语句前的分号&#8221;;&#8221;删除，具体如下：

;extension=php\_gd2.dll 改为extension=php\_gd2.dll

;extension=php\_mbstring.dll 改为extension=php\_mbstring.dll

;extension=php\_mysql.dll 改为extension=php\_mysql.dll

;extension=php\_mysqli.dll 改为extension=php\_mysqli.dll

;extension=php\_pdo\_mysql.dll改为extension=php\_pdo\_mysql.dll

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur14.jpg) 

然后搜索extension\_dir，修改路径为extension\_dir = &#8220;C:\inetpub\php\ext\&#8221; ，同时将前面的分号&#8221;;&#8221;删除生效。

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur15.jpg) 

10、PS：(在命令行中进入php安装目录下,比如C:\inetpub\php\php.exe -m，输入php -m命令，即可查看已开启的dll扩展模块)。

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur16.jpg) 

**三、部署MySQL数据库  
** 

由于PHP网站大多数依赖MySQL数据库，因此，我们还得手动部署数据库套件和服务，这时，我们只需下载安装MySQL数据库套件，就自动联机PHP+IIS环境。

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur17.jpg) 

**阿象提醒**：在MySQL安装过程中，建议设置&#8221;Server Machine（服务器）&#8221;模式，默认端口为3306，同时也要为root管理员设置高强度的密码。

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur18.jpg) 

**四、本地测试PHP程序  
** 

现在，我们只需将PHP论坛程序手动部署在C:\inetpub\wwwroot目录下，即可安装、运行、调试PHP网站，如下图所示；

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur19.jpg) 

**五、域名绑定、DNS解析  
** 

当PHP论坛完成调试后，我们即可将Azure虚拟机公网IP绑定域名，开启DNS解析服务，例如国内DNSPod服务商，即可完成网站后续工作，支持外网访问解析。

&nbsp;

**1、为什么Azure虚拟机支持绑定域名？  
** 

阿象：这是由于Azure为每个虚拟机分配独立公网IP，也就是服务器IP地址，从而实现建站目标，具体在仪表板进行查询。

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur20.jpg) 

**2、如何解析域名和DNS？  
** 

阿象：Azure玩家需要准备一个域名，例如xiang8.tk，具体可以用DNSPod域名解析服务，手动添加Azure公网IP两条A记录，即可完成网站解析服务。

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur21.jpg) 

**3、外网如何访问我的Azure虚拟机本地网站？  
** 

阿象：这个非常简单。直接输入IP+网站根目录，或者域名+网站根目录，即可。例如阿象随机搭建一个演示站：<a href="http://www.xiang8.tk/bbs" target="_blank"  rel="nofollow" >http://www.xiang8.tk/bbs</a> （延迟在0.020秒左右，速度非常惊人）

![](http://www.axiangblog.com/wp-content/uploads/2014/08/081214_1554_WindowsAzur22.jpg) 

**阿象点评**：Azure虚拟机建站非常适合新手、老手站长，整体体验就是Windows完全本地化测试，依赖IIS+PHP+MySQL三大件，操作非常简洁明了，同时Azure服务器提供了四核心、28G内存以及140GB流量额，这道&#8221;免费午餐（可试用60天）&#8221;非常诱人。