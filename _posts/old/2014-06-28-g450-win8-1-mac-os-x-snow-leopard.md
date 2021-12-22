---
id: 5013
title: 阿象玩黑苹果：联想G450 Win8.1安装Mac OS X Snow Leopard雪豹
date: 2014-06-28T16:09:14+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=5013
permalink: /g450-win8-1-mac-os-x-snow-leopard.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "28828"
baidu_record:
  - "1"
bigfa_ding:
  - "5"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:5012;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_2:
  - "3"
smilie_vote_1:
  - "2"
love:
  - "1"
categories:
  - Win10
  - Win8.1
  - 未分类
---
距离上次装黑苹果已过去两年，期间也先后安装多次系统，同时也对老本G450折腾改造升级，最关键的是装备240G SSD固态硬盘、英特尔E8135处理器。因此，阿象决定重温黑苹果那段折腾岁月，直接体验PC安装黑苹果系统的乐趣，下面阿象也整理个人如何在Win8.1平台安装Mac OS X 10.6.3雪豹系统图文过程，欢迎更多G450用户加入黑苹果队伍。 

下面是本次的主角——联想G450-TFO系列，只要类似相同配置的显卡、声卡、网卡（有线与无线），即可完美安装体验黑苹果系统。熟悉黑苹果的童鞋都明白这样的道理，不怕装不上黑苹果，最怕装完后没有驱动支持，尤其遇到没声音，没显卡加速特性，没网卡支持，那才是永远的痛。 

附阿象联想G450升级前后配置： 

**CPU：Pentium T4400 @ 2.20GHz（已升级Core 2 E8135 @ 2.66GHz）  
** 

**内存：2 GB+4GB  
** 

**硬盘：240G SSD固态硬盘+1TB 7200转 日立硬盘  
** 

**主板：联想NITU1 (英特尔4 Series–ICH9M+GM45芯片组  
** 

**显卡：Nvidia GeForce G210M 512MB  
** 

**声卡：Conexant Cx20561 @ Intel 82801IB ICH9 – High Definition Audio Controller  
** 

**网卡：博通 BCM5906M NetLink Fast Ethernet  
** 

**无线网卡：博通BCM4310  
** 

**电池: LGPABAS024  
** 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W1.png) 

最后效果：睡眠不能唤醒。其他驱动完美（声卡，显卡，有线无线网卡等等）。连wifi无线上网也可以用。先晒一下阿象的成果。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W2.png) 

 

**准备工作：  
** 

1、原版苹果**Mac.OS.X.10.6.3.Retail.dm**g镜像； 

<p style="margin-left: 11pt">
  2、<strong>变色龙Chameleon</strong> ，具体分Windows、Mac版本]，支持引导Win7、Win8、Win8.1、Mac OS X以及Linux系统，安装卸载都比较方便。
</p>

3、第三方WinPE或者Win7、Win8.1原版镜像U盘启动盘（主要为了设置C盘为活动分区用），推荐第三方WinPE工具； 

4、**硬盘安装助手**，主要用于写入苹果dmg镜像； 

5、磁盘工具**DiskGenius**：用于设置引导和分区标记（具体区分下载32和64位版本）； 

6、Mac.OS.X.10.6.3.Retail内核替换文件OSInstall，用于破解内核：注：替换文件是让苹果系统可以安装在MBR分区上，即Windows分区。 

7、**HFS Explorer**和Java（Java平台），先安装Java，才能正常使用HFS Explorer。 

8、**Macdrive 9**以及注册机，以及对于win8.1 64位的驱动补丁patch 

**全文所有工具可以到这里下载：  
** 

<a href="http://pan.baidu.com/s/1dDkrYzZ" target="_blank"  rel="nofollow" >http://pan.baidu.com/s/1dDkrYzZ</a>、 <a href="http://www.400gb.com/u/2574829/4214372" target="_blank"  rel="nofollow" >http://www.400gb.com/u/2574829/4214372</a> 

 

**具体步骤：**（以Win8.1为例）**  
** 

**第一步：准备2个空白分区**（千万别格式化） 

1、使用组合键Win+X，或右击开始按钮，打开磁盘管理； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W3.jpg) 

2、选择磁盘最后一个分卷，确保有30G左右（或更大）剩余空间，然后右键选择压缩卷， 例如压缩量为37888（37G），其中：7G用于建立Mac OS X安装盘，30G用于苹果系统分区； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W4.jpg) 

3、等待压缩完毕后，自动生成37G未分配空间，继续右键选择新建简单卷，填入7168（7G），用来安装雪豹系统，然后下一步； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W5.jpg) 

注：可分配盘符，但是不能格式化，尤其新建分卷后，系统会再提示是否格式化，直接取消。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W6.jpg) 

4、随后，我们直接将剩下未分配的分区新建简单卷，操作步骤同上，也不能格式化！！ 

 

**第二步：提取安装镜像、写入分区、替换内核  
** 

1、重新提取DMG系统镜像 

首先对Mac OS X 10.6.3原版苹果系统镜像开刀：使用HFS Explorer加载重新提取打包DMG镜像，选择+HFS苹果专属磁盘格式，去掉麻烦的引导层部分，以便硬盘安装助手能识别。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W7.jpg) 

然后重新生成新的DMG镜像，如下图所示，选择Create disk image。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W8.jpg) 

2、写入dmg到安装分区 

下面，打开以管理员身份运行&#8221;硬盘安装助手&#8221;，只需勾选&#8221;写入&#8221;，另外三项不选，选择之前创建的7G安装分区，如图： 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W9.jpg) 

接着等待写入任务完成，阿象建议这时别弄电脑，否则会出现假死（表面上进度条不动，其实写入还在进行） 

当出现**Change Partition type to AF: success**就写入成功；当出现**Change Partition type to AF: failed**，可以使用 DiskGenius将分区的系统标识，更改分区参数AF，如图所示： 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W10.jpg) 

3、替换OS X内核文件： 

安装Macdrive 9.2，就可在Win8.1下直接访问、读写Mac分区（Mac安装盘、Mac系统盘等）。阿象注：首次安装完Macdrive需要重启电脑，才能访问Mac分区。 

这时，直接打开Mac安装分区，同时显示隐藏文件，分别替换如下两个内核破解文件： 

一、OSInstall文件路径： 

/System/Library/PrivateFrameworks/Install.framework/Frameworks/OSInstall.framework/ 

Versions/A/，覆盖替换原文件。 

二、OSInstall.mpkg文件路径 ：/System/Installation/Packages，替换原文件 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W11.jpg) 

 

**第三步：安装变色龙  
** 

下面，我们在Win8.1平台直接安装变色龙Chameleon Install for Windows][变色龙安装程序]，支持自定义主题、英语或简体中文，然后选择右侧的安装，或者卸载。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W12.jpg) 

装完Chameleon变色龙引导后，我们还得提前准备Kext文件，防止G450灰苹果、无限风火轮情况，具体将（标记**安装盘**）Extensions文件夹全部放在安装分区的目录/Extra/Extensions（没有这个文件夹请自行新建Extra） 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W13.jpg) 

**第四步：开始安装Snow Leopard  
** 

重启Win8.1，选择Chameleon引导，移动光标至MAC OS X install DVD，回车，即可进入欢迎界面。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W14.jpg) 

然后选择工具栏上的磁盘工具，点击Win8.1平台最后一个空白30G左右的分区(diskOS..)； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W15.jpg) 

阿象提醒：这个分区千万别选错，否则将彻底丢失Windows分区资料。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W16.jpg) 

接着选择**抹掉**、选择**Mac OS 扩展式 (日志式)**，重新命名系统盘名称，例如macosx，注意，名称要用英文； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W17.jpg) 

当抹掉磁盘分区后，直接关闭该窗口，重新返回Mac OS X安装欢迎界面，选择**自定**，即可使用刚才的空白30G分区； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W18.jpg) 

在自定义选项中无需安装打印机支持，因为打印机相关文件比较大，安装完成后可以再从网上下载安装。X11、Rosetta选上，QuickTime 7可以不用安装。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W19.jpg) 

最后，我们G450本本成功完成Mac OS X 10.6.3安装任务。 

 

**第五步：激活Win8.1主分区  
** 

这时重启电脑后，我们会发现无法引导G450进入原来的Win8.1系统，这时我们需要恢复引导，即激活Win8.1主分区，具体可以使用WinPE工具。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W20.jpg) 

加装WinPE系统，打开DiskGenius，选择Win8.1系统的C盘，右键选择&#8221;激活当前分区&#8221;后保存更改，重启即可生效。 

 

**第六步，Mac OS X配置篇  
** 

在登陆Mac OS X之前，我们需要准备G450机型KEXT和DSDT，否则可能无法驱动声卡、网卡、显卡。而Kext可以为内核提供扩展，DSDT可以帮Mac OS X直接读取BIOS信息，同时可以驱动显卡、声卡和网卡，其过程比使用Kext要繁琐，而回报是使你电脑更像苹果原型Mac。使用DSDT工具生成 DSDT.aml后放在变色龙的/Extra下面就能实现DSDT改写。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W21.jpg) 

具体只需在Mac OS X系统分区里面新建Extra文件夹，将Extensions放入其中，包括dsdt.aml，稍后即可重启 

 

**第七步：个性化Mac OS X  
** 

重启G450，切换变色龙启动，选择Mac OS X系统分区，回车。第一次进入苹果系统有点慢，等待一下就能看到苹果欢迎动画。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W22.jpg) 

接下来就是一些Mac OS X设置，非常类似Win8.1个性化，具体包括创建计算机名称、你的账户、系统时区等内容。. 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W23.jpg) 

在设置时区时，请选择中国北京，稍后要安装Mac时间同步补丁（在mac中直接安装就可以了），不然Win8.1将会出现时间差问题。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W24.jpg) 

设置完就进入了苹果的华丽的桌面，正常情况下,声卡，显卡，有线和无线网卡，电池可以识别使用，人品好的话，触控板也是可以使用了,还可以使用点击功能;如果还没检测到,建议重启,选变色龙,然后移动到你的mac系统盘的上 ,按-f 加载驱动。 

如果你需要手动更新声卡、网卡和显卡驱动，只需重新加入kext文件和dsdt解决，然后借助以下两个pkg软件进行权限的修复：左边是修复权限，右边为安装kext驱动的工具。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062814_1609_G450W25.png) 

阿象提醒：**如果显卡驱动正常工作，这时将支持水纹特效，同时在系统偏好设置可以选择声卡输出，但需要手动切换耳机、扬声器**。 

**第八步：更新至Mac OS X 10.6.8  
** 

关于更新，苹果公司分别提供在线更新、离线Combo升级包。阿象推荐离线升级，同时逐一更新，不建议从10.6.3直接升级到10.6.8。比如，借助Mac OS X Upd Combo 10.6.6升级到10.6.6，然后升级至Mac OS X Upd 10.6.7、Mac OS X Upd 10.6.8。 

注：阿象实际操作发现从Mac OS X 10.6.3直接升级到10.6.8，这时G450显卡驱动就崩溃，出现黑屏。 

附Mac OS X 10.6.x各种升级包的下载： 

MacOSXUpdCombo10.6.6安裝包（适合10.6.1-10.6.5任一平台） 

<a href="http://supportdownload.apple.com/download.info.apple.com/Apple_Support_Area/Apple_Software_Updates/Mac_OS_X/downloads/041-4905.20110106.ARe3a/MacOSXUpdCombo10.6.6.dmg" target="_blank"  rel="nofollow" >http://supportdownload.apple.com/download.info.apple.com/Apple_Support_Area/Apple_Software_Updates/Mac_OS_X/downloads/041-4905.20110106.ARe3a/MacOSXUpdCombo10.6.6.dmg</a> 

 

MacOSXUpd10.6.7升级包（只能在10.6.6上面运行） 

<a href="http://supportdownload.apple.com/download.info.apple.com/Apple_Support_Area/Apple_Software_Updates/Mac_OS_X/downloads/041-4916.20110321.Sx74f/MacOSXUpd10.6.7.dmg" target="_blank"  rel="nofollow" >http://supportdownload.apple.com/download.info.apple.com/Apple_Support_Area/Apple_Software_Updates/Mac_OS_X/downloads/041-4916.20110321.Sx74f/MacOSXUpd10.6.7.dmg</a> 

 

MacOSXUpd10.6.8升级包（只能在10.6.7上面运行） 

<a href="http://supportdownload.apple.com/download.info.apple.com/Apple_Support_Area/Apple_Software_Updates/Mac_OS_X/downloads/041-4961.20110725.GqHgj/MacOSXUpd10.6.8.dmg" target="_blank"  rel="nofollow" >http://supportdownload.apple.com/download.info.apple.com/Apple_Support_Area/Apple_Software_Updates/Mac_OS_X/downloads/041-4961.20110725.GqHgj/MacOSXUpd10.6.8.dmg</a> 

 

 