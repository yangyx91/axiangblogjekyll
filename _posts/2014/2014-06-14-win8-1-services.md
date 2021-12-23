---
id: 4783
title: 我的系统我做主，如何手动优化Win8.1系统服务、任务计划程序？
date: 2014-06-14T08:59:39+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=4783
permalink: /win8-1-services.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "30161"
baidu_record:
  - "1"
bigfa_ding:
  - "5"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:4782;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_6:
  - "2"
smilie_vote_5:
  - "1"
smilie_vote_2:
  - "1"
categories:
  - Win10
  - Win8.1
  - 未分类
---
近期，阿象分享个人使用心得，帮助大家<a href="http://www.axiangblog.com/win7-win8-1-good-habits.html" target="_blank" rel="nofollow" >养成Win7、Win8.1好习惯，告别重装系统</a>的烦扰。这次，阿象继续带大家学习下如何手动优化Win8.1系统服务、任务计划程序等攻略，真正做到我的系统我做主，明明白白玩优化。

从Win7、Win8.1开始，微软为我们带来完善的系统服务、任务计划程序，这些都一定程度提升了日常使用，实现了&#8221;半自动化、半智能化&#8221;交互体验。但是对于高级用户来说，这些所谓的任务计划程序、系统服务、系统后台程序可以切换成手动模式或禁用，尤其对于机械硬盘用户来说，有着明显的速度提升。

注：这次系统优化前提也是因人而异，毕竟童鞋们机器配置、软件环境有差异，因此，阿象以个人使用经历参考示范，抛砖引玉供大家参考。

**一、启动项  
** 

启动项，也叫开机启动项，相信这个大家比较熟悉，减少开机自启动的程序应用，可以大幅提升开机速度。

最新Win8.1引入全新的任务管理器（如下图），切换至启动项，即可查看当前已启用、已禁用的开机应用程序。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061414_0859_W1.jpg) 

例如阿象Win8.1平台已启用3个开机启动程序，其他均手动禁用，具体操作也非常简便，只需右击目标程序，选择禁用。

如果你是Win7用户，操作略繁琐，即Win+R组合键打开运行，输入msconfig，在Win7当前的系统设置，同样可以手动禁用开机启动项。

**二、Win8.1磁盘优化  
** 

从Win8、Win8.1开始，微软为机械硬盘、固态硬盘引入&#8221;磁盘优化&#8221;计划程序，取代了原先的传统磁盘碎片整理概念。虽然微软好意加入功能，但对于机械硬盘用户来说，这项计划任务有时严重影响自己上网、游戏或者办公等环境。

因此，阿象推荐关闭&#8221;优化驱动器&#8221;计划项目，改为不定期手动操作该功能。具体依次打开：控制面板\系统和安全，选择优化驱动器，禁用计划运行。（如下图）

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061414_0859_W2.jpg) 

**三、Win8.1客户体验计划  
** 

从Win8.1开始，微软默认为用户开启&#8221;参与Windows客户体验改善计划&#8221;，回收Win8.1各种错误代码、硬件兼容性、软件运行出错等数据资料。如果童鞋们比较在意个人隐私，不愿意将自己的Win8.1使用习惯分享给微软大叔，也可以直接拒绝参加体验计划。

具体操作如下：依次打开：控制面板\系统和安全\操作中心\更改操作中心设置，选择&#8221;客户体验改善计划&#8221;，更改为&#8221;我不想参与该计划。&#8221;

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061414_0859_W3.jpg) 

**四、任务计划程序  
** 

下面进入今天的主角之一：任务计划程序。（普通用户直接打开&#8221;这台电脑&#8221;，选择顶部功能区的&#8221;管理&#8221;，即可快速进入&#8221;计算机管理&#8221;）

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061414_0859_W4.jpg) 

其中任务计划程序主要有三大类：Microsoft、OfficeSoftwareProtectionPlatform、WPD；Microsoft旗下有三类子栏目，即Office、Windows、Windows Live。

下面是阿象个人具体手动禁用的Win8.1任务计划程序，参考如下：（Win7童鞋们可以参考优化）

**1、OfficeSoftwareProtectionPlatform：  
** 

SvcRestartTask //具体是Office相关服务，建议禁用

**2、Microsoft（Office子栏目）：  
** 

Office Automatic Updates //Office自动更新服务，建议禁用

**3、Microsoft（Windows子栏目）：  
** 

.NET Framework //内置四项任务计划，可禁用

Application Experience //主要功能为参与Microsoft 客户体验改善计划，其分支AitAgent和ProgramDataUpdater两项禁用

Autochk //又是Microsoft 客户体验改善计划，果断禁用

Bluetooth //蓝牙，有蓝牙设备的童鞋就略去；没蓝牙的童鞋，果断禁用

Chkdsk //主要用于不定期NTFS卷状况扫描，可禁用

Customer Experience Improvement Program//人如其名，这也是一项的标准的Microsoft 客户体验改善计划，其四项子项目BthSQM、Consolidator、KernelCeipTask、UsbCeip，也可以果断禁用

Data Integrity Scan //其中Data Integrity Scan任务将扫描容错卷的潜在损坏，可禁用

Defrag //其中ScheduledDefrag任务将优化本地存储驱动器，推荐禁用

Diagnosis //其中Scheduled任务属于Windows计划的维护任务，如果嫌这个烦人的提示，就禁用吧

DiskDiagnostic //也是一项Microsoft 客户体验改善计划，其中两项子任务均可禁用，即Microsoft-Windows-DiskDiagnosticDataCollector、Microsoft-Windows-DiskDiagnosticResolver

Maintenance //其中WinSAT任务将测量系统的性能和功能，可以禁用

Media Center //即媒体中心Media Center，还是自主决定吧，阿象也时常会用下Media Center，可以留着

Offline Files //当用户在脱机模式下工作时，此任务控制脱机文件的定期后台同步，可禁用其中Background Synchronization、Logon Synchronization任务

PerfTrack // 其BackgroundConfigSurveyor任务属于性能跟踪空闲任务: 后台配置调查程序，禁用

RAC //其RacTask任务将用于处理系统可靠性数据，禁用

TaskScheduler //其中Idle Maintenance、Manual Maintenance两项任务计划可禁用

Windows Media Sharing //其中UpdateLibrary任务可更新用户共享媒体库中缓存的文件夹列表和所有新文件的安全权限，可以禁用

WindowsBackup———–系统备份，———–这个还是禁用吧，如果要备份，还是手动放心些。

至于其他未列出的计划服务项目，就要靠童鞋们的火眼金睛去发现优化了，做到因人而异了，不过阿象建议动手能力较差的童鞋们，其他项目还是不要优化了，除非是十拿九稳的计划程序，才能果断禁用。

&nbsp;

**五、Win8.1系统服务  
** 

由于阿象水平，境界都比较低，只能以日常使用中的经验来叙述，如果不全面，喜欢童鞋们及时补充，反馈。。。。。。

1、Alipay security service

//-为支付宝安全产品提供服务，习惯网购，这个就比较熟悉，默认是自动，可以设置手动

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061414_0859_W5.jpg) 

2、Background Intelligent Transfer Service

//使用空闲网络带宽在后台传送文件—-这个可以手动，或者禁用吧

3、BitLocker Drive Encryption Service

//这个是属于Win8.1企业版的BitLocker 驱动器加密服务，手动，或者禁用

4、Bluetooth Support Service

//与前面相似，有没有蓝牙设备，自主选择，自动，手动或者禁用

5、IP Helper

//针对于使用 IPv6 转换技术，如果还是ipv4的童鞋，可以设置为手动，或者自动（延迟）

6、Program Compatibility Assistant Service

//-程序兼容性助手(PCA)，如果厌烦其不断地提示，可以手动或者禁用

7、Security Center

//安全中心，监测系统健康状态，可以手动，或者禁用

8、Windows Search

//系统搜索索引，如果有SSD固态硬盘的童鞋可以禁用。

9、Superfetch

//维护和提高一段时间内的系统性能，如果有SSD固态硬盘的童鞋可以禁用

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061414_0859_W6.jpg) 

10、第三方软件服务项

例如Google Chrome自动更新、VMware所有组件等服务需要靠童鞋们的火眼金睛去手动优化。

当然还是那句话，Win8.1系统优化因人而异。最后阿象也建议动手能力较差的童鞋们，其他项目还是不要优化了，除非是十拿九稳的系统服务，才能禁用，否则就更改为手动启动，即可。