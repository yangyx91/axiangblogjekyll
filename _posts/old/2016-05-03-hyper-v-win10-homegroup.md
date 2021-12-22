---
id: 9459
title: Hyper-V、物理机传文件很简单，巧用Win10家庭组本地共享文件
date: 2016-05-03T10:33:34+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=9459
permalink: /hyper-v-win10-homegroup.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "49835"
baidu_record:
  - "1"
love:
  - "9"
smilie_vote_1:
  - "3"
smilie_vote_4:
  - "4"
smilie_vote_3:
  - "4"
smilie_vote_2:
  - "5"
smilie_vote_5:
  - "3"
smilie_vote_6:
  - "3"
categories:
  - Web开发
  - Win10
  - 未分类
---
从事Windows开发的童鞋，经常离不开Hyper-V虚拟机管理器产品，尤其是调试各类Win10 UWP应用和游戏，不过由于Hyper-V本身限制，无法直接与物理机互相传文件。不过我们可以曲线使用Win10家庭组（类似XP时代的网上邻居），直接在本地局域网内，互相传输文件。

下面，笔者也简单分享下Win10 Pro专业版、Win10企业版下如何搭建家庭组，共享Hyper-V本地文件和资料，参考如下：

<a href="http://www.axiangblog.com/hyper-v-win10-homegroup.html/hyper-homegroup1" rel="attachment wp-att-9460" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9460" src="http://www.axiangblog.com/wp-content/uploads/2016/05/hyper-homegroup1.jpg" alt="hyper-homegroup1" width="500" height="326" /></a>1、首先在物理机（本机环境），打开Win10《设置》，进入网络和Internet栏目，选择“家庭组”

<a href="http://www.axiangblog.com/hyper-v-win10-homegroup.html/hyper-homegroup2" rel="attachment wp-att-9461" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9461" src="http://www.axiangblog.com/wp-content/uploads/2016/05/hyper-homegroup2.jpg" alt="hyper-homegroup2" width="500" height="369" /></a>

2、根据家庭组的提示，手动“更改网络位置”为“**家庭和工作网络**”，非公共网络，即可；

<a href="http://www.axiangblog.com/hyper-v-win10-homegroup.html/hyper-homegroup3" rel="attachment wp-att-9462" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9462" src="http://www.axiangblog.com/wp-content/uploads/2016/05/hyper-homegroup3.jpg" alt="hyper-homegroup3" width="500" height="314" /></a>3、继续**创建家庭组**，系统默认共享图片、视频、音乐、文档以及打印机等设备；

<a href="http://www.axiangblog.com/hyper-v-win10-homegroup.html/hyper-homegroup4" rel="attachment wp-att-9463" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9463" src="http://www.axiangblog.com/wp-content/uploads/2016/05/hyper-homegroup4.jpg" alt="hyper-homegroup4" width="500" height="265" /></a>4、家庭组默认会生成一个唯一的密码，用于其他PC的安全验证和访问，用于接入当前家庭组；

<a href="http://www.axiangblog.com/hyper-v-win10-homegroup.html/hyper-homegroup5" rel="attachment wp-att-9464" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9464" src="http://www.axiangblog.com/wp-content/uploads/2016/05/hyper-homegroup5.jpg" alt="hyper-homegroup5" width="500" height="256" /></a>5、家庭组默认共享个人文件夹，不过我们手动共享其他本地文件夹和资料，比如新建一个“我的软件”文件夹，存储需要传送到Hyper-V虚拟机的工具或资料，在窗口工具栏选择共享到“家庭组（查看）”或者““家庭组（查看和编辑）”，完成共享任务；

<a href="http://www.axiangblog.com/hyper-v-win10-homegroup.html/hyper-homegroup6" rel="attachment wp-att-9465" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9465" src="http://www.axiangblog.com/wp-content/uploads/2016/05/hyper-homegroup6.jpg" alt="hyper-homegroup6" width="500" height="273" /></a>6、最后我们进入Hyper-V虚拟机，加入家庭组，就可以访问物理机上共享的文件夹，比如“我的软件”里的工具和资料；

<a href="http://www.axiangblog.com/hyper-v-win10-homegroup.html/hyper-homegroup7" rel="attachment wp-att-9466" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9466" src="http://www.axiangblog.com/wp-content/uploads/2016/05/hyper-homegroup7.jpg" alt="hyper-homegroup7" width="450" height="373" /></a>

7，当然，我们也可以手动停止共享这些文件夹、或者共享其他新文件夹。