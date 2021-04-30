---
id: 4804
title: Win8.1也能随身带，如何打造Windows To Go版Win8.1 U盘系统
date: 2014-06-16T14:17:19+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=4804
permalink: /windows-to-go-win8-1.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "56473"
baidu_record:
  - "1"
bigfa_ding:
  - "6"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:4803;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_1:
  - "9"
smilie_vote_2:
  - "10"
smilie_vote_4:
  - "2"
smilie_vote_5:
  - "3"
smilie_vote_3:
  - "3"
love:
  - "1"
smilie_vote_6:
  - "1"
  - "1"
categories:
  - Win10
  - Win8.1
  - 未分类
---
从Windows XP一直到Win7，我们常常认为Windows系统只能安装在本地硬盘，无法打造一个U盘系统。当然，民间爱好者也为大家贡献了各种Win2003、Win7内核的PE系统，实现U盘系统概念。但是这些PE系统只能充当一个临时系统环境，不具有Windows所有正常功能。

好在微软在Win8、Win8.1中带来一项全新的Windows To Go功能，原生支持将Win8.1专业版、企业版系统安装至可移动U盘、移动硬盘等移动设备，真正打造一款移动版Win8.1系统。

这也意味着用户可以在任何一台支持USB接口的公共电脑、平板电脑设备上直接启动运行U盘版Win8.1系统，单独享用个人专属系统，包括桌面、收藏夹、个人数据等资料。

当然，Windows To Go功能不仅可以打造移动U盘系统，同时也可以取代传统PE系统工具，直接参与到系统维护、修复计算机、数据备份还原等领域。

长话也不多说，下面阿象也整理了如何打造Windows To Go版Win8.1个性U盘系统完整图文教程，欢迎Win8.1新老用户体验。

**准备工具：**Win8.1 with Update MSDN ISO系统镜像（<a href="http://www.axiangblog.com/win8-1-resource-summary.html" target="_blank" rel="nofollow" >点击这里下载</a>），不限企业版、专业版；imagex 6.3.9600映像管理工具（<a href="http://pan.baidu.com/s/1mgwUJyw" target="_blank" rel="nofollow" >点击下载</a>）；大容量U盘，至少16G及以上，推荐32G U盘。

**测试平台：**Win8.1 Update环境

**操作步骤：  
** 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win811.jpg) 

注：其中Win8.1企业版自带了Windows To Go组件，但Win8.1专业版、核心版未内置该组件，因此我们可以使用命令提示符，手动创建一个Windows To Go版Win8.1个性U盘。

1、使用虚拟光驱（Win8.1自带）加载Win8.1 ISO镜像，复制X：\sources\install.wim至本地磁盘，例如E：\Win8（其中X：代表虚拟光驱盘符）；

&nbsp;

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win812.jpg)![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win813.jpg) 

2、解压Imagex 6.3.9600中的x86版本的imagex.exe（如下图所示）至本地硬盘，例如E：\Win8；

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win814.jpg) 

3、然后访问本地系统盘C：\Windows\System32目录，复制bcdboot.exe（如下图所示）至本地硬盘，例如E：\Win8；

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win815.jpg) 

&nbsp;

4、随后右击Win8.1传统桌面的开始按钮（或组合键Win+X），打开&#8221;命令提示符（管理员）&#8221;，打开命令运行框；

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win816.jpg) 

&nbsp;

5、依次输入如下命令：

**Diskpart** // 计算机磁盘管理

**List disk** // 显示当前所有本地硬盘、可移动硬盘

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win817.jpg) 

例如阿象电脑是SSD+HDD双硬盘，外接一个U盘，其中U盘标记为磁盘2，具体以实际情况为例。

6、下面我们要对U盘重新分区、激活分区，继续输入如下命令：

**Select disk 2** //选择当前U盘，具体以实际情况为例

**Clean** //清除U盘数据

**Create partition primary** //创建主分区

**Select partition 1** //选择当前U盘分区

**Format fs=ntfs quick** //启动快速格式化，默认格式为NTFS磁盘格式

**Active** //激活U盘分区为活动区

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win818.jpg) 

7、关闭命令符窗口，分别将之前E：\win8目录下的imagex、bcdboot.exe两项系统工具复制到当前移动U盘下。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win819.jpg) 

8、继续打开&#8221;命令提示符：管理员&#8221;，使用命令定位当前U盘目录，具体命令如下：

**X：** // 这里的X代表当前U盘盘符，具体以实际情况为主

**imagex.exe /apply e:\win8\install.wim 1 X:\** //即将原e:\win8\install.wim映像部署到U盘

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win8110.jpg) 

然后等待Windows To Go版Win8.1制作完成，具体时间取决于USB接口、U盘写入速度。当命令框提示Successfully applied image时，即操作已完成。

&nbsp;

9、当上一操作完成后，继续在命令框中输入命令，具体如下：

**Bcdboot.exe X:\Windows /s X: /f all** //这里的X代表U盘，并设置U盘系统启动项并激活

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win8111.jpg) 

当命令框提示Bootfiles successfully created（已成功创建启动文件）时，即操作已完成。

&nbsp;

10、重启电脑，设置BIOS引导，切换至USB引导模式，一般直接使F12，即可快速更改至U盘启动模式。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win8112.jpg) 

这时，我们将看到Win8.1开始初始化，正在准备设备，

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win8113.jpg) 

首次运行Win8.1时间会比较慢，然后个性化Win8.1。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win8114.jpg) 

最后，我们成功创建一个Windows To Go版Win8、Win8.1专属U盘系统，如下图所示。其中U盘成为Win8.1默认系统盘，实际占用体积大约在6G左右。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1417_Win8115.jpg) 

注：阿象分别用16G U盘测试Win8、Win8.1两个企业版系统，其中Win8.1最低硬件要求至少32G U盘，不支持16G U盘。

因此，如果你只有16G U盘，建议优先安装体验Windows To Go版Win8系统；或者升级32G大容量U盘，即可安装体验Win8.1 Update平台。

&nbsp;