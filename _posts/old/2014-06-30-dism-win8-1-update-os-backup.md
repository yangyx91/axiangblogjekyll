---
id: 5042
title: 抛弃Ghost，自己动手制作Win8.1/Win8.1 Update出厂恢复镜像
date: 2014-06-30T15:35:40+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=5042
permalink: /dism-win8-1-update-os-backup.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "76589"
baidu_record:
  - "1"
bigfa_ding:
  - "10"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:5041;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_1:
  - "11"
smilie_vote_2:
  - "9"
smilie_vote_6:
  - "2"
smilie_vote_4:
  - "3"
smilie_vote_3:
  - "1"
love:
  - "1"
categories:
  - Win10
  - Win8.1
  - 未分类
---
进入2014年，不少品牌笔记本、超极本、台式机开始预装Win8.1正版系统，虽然Win8.1褒贬不一，但不能阻止微软的开发进度，例如4月份的 Win8.1 Update，8月份的Win8.1 Update2，还有2015年的Win8.1 Update3，很显然2014、2015年主旋律依旧是Win8.1，或者说是Win8.1时代。

由于微软取消在大陆市场的Win8/Win8.1实体光盘销售，因此品牌电脑厂商常常为Win8.1电脑中附带一个出厂恢复镜像。当用户遇到系统股长、崩溃时，只需恢复出厂、重装系统就可以顺利解决问题。

但Win8.1 Update发布后，品牌机器预装的出厂恢复镜像依旧是2013年旧款Win8.1系统，因此每次恢复出厂后，普通用户还要重新升级至Win8.1 Update平台，为何不自己手动制作Win8.1 Update出厂恢复镜像？当然组装机、普通品牌机（裸机）用户也可以自己动手，制作个性化出厂恢复镜像，提前预防。

幸好Win8、Win8.1分别引入三套全新的**系统恢复**方案，1、恢复电脑而不影响你的文件（类似系统修复）；2、恢复所有内容并重新安装Windows（类似系统重装、出厂设置）；3、高级启动（类似Win7时代高级启动菜单）。因此，我们直接个性化出厂恢复镜像。下面，阿象也为普通Win8.1爱好者整理了如何动手制作Win8.1/Win8.1 Update出厂恢复镜像图文教程，具体如下：

**准备工具：**Win8.1 With Update MSDN原版ISO系统镜像（<a href="http://www.axiangblog.com/win8-1-resource-summary.html" target="_blank"  rel="nofollow" >点击这里下载</a>）

**测试环境：**Win8.1平台

**阿象点评：**以往系统重装时，我们常常需要刻录光盘、制作U盘启动、或者PE等安装方式，不过Win8.1引入Windows修复环境 (Windows RE)恢复还原工具，因此，我们可以直接创建隐藏分区、制作Win8.1 Update出厂恢复镜像，既可以在本地硬盘上恢复，无需光盘、U盘等传统介质。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW1.jpg) 

1、提前安装Win8.1 Update更新、各类显卡驱动、常用软件等程序；

2、组合键Win+X，打开磁盘管理，单独划分一个分区，例如X盘，主要用于存放Win8.1、Win8.1 Update出厂恢复镜像；（可设置隐藏，类似品牌机型的一键还原）

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW2.jpg) 

3、加载Win8.1 With Update MSDN原版ISO镜像，定位至其目录下/sources/install.wim，将其复制到非系统盘，例如X:\Restore，另外还需新建一个缓存文件夹，如X:\Temp；

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW3.jpg) 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW4.jpg) 

4、组合键Win+I，打开Modern版**电脑设置》更新与恢复功能》恢复》高级启动**，重新启动Win8.1平台；

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW5.jpg) 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW6.jpg) 

5、重启电脑后，系统将进入修复环境（Windows RE），这时选择**疑难解答》高级选项》命令提示符**，验证个人账户，打开**命令提示符**窗口；

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW7.jpg) 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW8.jpg) 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW9.jpg) 

6、用Diskpart命令检查以下Install.wim映像文件、temp缓存文件、当前Win8.1系统盘主分区的实际物理路径。

**具体可以执行如下命令：  
** 

**Diskpart** //进入Diskpart界面

**list disk** //显示当前电脑本地磁盘

**select disk N** //选中Win8.1所在的磁盘N

**list part** //显示磁盘N本地分区

**select part N** //选择分区N

**detail partition** //显示分区N的详情内容

**Exit** //退出Diskpart界面

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW10.jpg) 

经过查询后，由于当前Win8.1系统生成了350MB临时分区，因此当前的Win8.1系统盘主分区的驱动器盘符更改为D，即&#8221;C盘&#8221;，同时也确定其他分区的盘符。

&nbsp;

7、在命令提示符中键入Win8.1/Win8.1 Update系统盘备份映像命令：

**Dism /append-image /imagefile:X:\Restore\install.wim /scratchdir:X:\Temp /capturedir:Y:\ /Name:Windows8.1Backup  
** 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW11.jpg) **  
** 

//ImageFile:指定了Install.wim映像的完整路径；/ScratchDir：指定了自定义的缓存文件夹路径；/CaptureDir：指定了需要备份系统映像所在主分区的位置或者磁盘；/Name：表示的是wim格式的备份映像的名称。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW12.jpg) 

阿象测试，如果将当前29G体积Win8.1主分区制作为出厂设置镜像后，实际占用也只用到12G体积，压缩率非常优秀，值得一试。

&nbsp;

8、当备份完成后，可以使用如下命令查询install.wim系统映像：

**dism /get-wiminfo /wimfile:X:\Restore\install.wim  
** 

//查询install.wim映像的索引、名称

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW13.jpg) 

9、配置恢复映像工作，具体只需REAgentC命令，打开**命令符（管理员）**:

**reagentc /setosimage /path X:\Restore /index N  
** 

// path路径代表install.wim所在文件夹路径、index后面的N表示要恢复的wim映像中的索引号，例如选择index 3的Windows8.1Backup，当然也可以选择index 1。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW14.jpg) 

配置完成后，执行reagentc /info 命令，查看恢复映像配置情况，如上图所示。（需要注意Windows RE状态是否显示&#8221;Enable&#8221;）

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW15.jpg) 

10、开始初始化电脑。具体只需打开电脑设置》更新与恢复》恢复，选择**删除所有内容并重新安装Windows**，之后会出现下图提示：

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW16.jpg) 

选择下一步，用户可选&#8221;**仅删除我的文件**&#8220;（简单的格式化分区，初始化过程只需很少的时间，10分钟左右）；如果打算把电脑转让给他人，推荐选择第二个&#8221;**完全清理驱动器**&#8220;选项，这样恢复过程中会首先擦除分区以使分区中原有的文件难以再被恢复，这样需要的时间会比较长。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW17.jpg) 

11、最后一步，单击&#8221;**初始化**&#8220;后，Win8.1系统将自动重启，完成初始化，恢复出厂系统镜像状态。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW18.jpg) 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW19.jpg) 

整个初始化过程大概需要10分钟左右的时间，具体取决于你的硬盘速度、系统出厂镜像体积大小。当Win8.1完成初始化后，Win8.1还将再一次重启，进入硬件驱动配置，用户账户设置等操作，最后成功恢复到Win8.1/Win8.1 Update出厂镜像设置。

**阿象结语：  
** 

至此，我们才发现，无论是系统恢复或者重装，在Win8/Win8.1的时代，一切都变得如此简单化，可谓是&#8221;辛苦一次，造福万年&#8221;，真正实现无需外置光盘，或者U盘这类安装介质（如果只是&#8221;恢复电脑而不影响你的文件&#8221;，可借助安装盘或者U盘引导盘）。最后，欢迎各位Win8.1爱好者赶紧设置一下出产设置，以备不时之需。