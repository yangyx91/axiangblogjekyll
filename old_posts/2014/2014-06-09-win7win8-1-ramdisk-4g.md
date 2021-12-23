---
id: 4713
title: 给Win7/Win8.1提个速，如何安装设置RamDisk 4G虚拟内存盘？
date: 2014-06-09T15:47:37+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=4713
permalink: /win7win8-1-ramdisk-4g.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "25575"
baidu_record:
  - "1"
bigfa_ding:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:4711;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_4:
  - "2"
smilie_vote_1:
  - "1"
smilie_vote_5:
  - "1"
categories:
  - Win10
  - Win8.1
  - 未分类
---
<span style="font-family:宋体; font-size:10pt">对于普通64位Win7、Win8.1用户来说，常常将系统安装在机械硬盘上，因此在日常使用中难免遇到延迟、卡顿等问题，相应也影响了日常使用。<br /> </span>

<span style="font-family:宋体; font-size:10pt">如果你配置了4G以上的大内存，这时可以借助免费版RamDisk 4G工具轻松创建虚拟内存盘（RamDisk），充分利用内存高速读写的优势，将日常系统、常用应用程序的临时文件、缓存目录设置到RamDisk，从而实现为系统提速的效果。阿象也整理了RamDisk 4G详细的设置教程，参考如下：<br /> </span>

<span style="font-family:宋体; font-size:10pt">RamDisk 4G英文版官方最新版下载，6.3MB：（<a href="http://memory.dataram.com/products-and-services/software/ramdisk" target="_blank"  rel="nofollow" >访问官网</a>）<br /> </span>

<a href="http://memory.dataram.com/__downloads/memory/ramdisk/Dataram_RAMDisk_4_4_0_RC31.msi" target="_blank"  rel="nofollow" ><span style="font-family:宋体; font-size:10pt">http://memory.dataram.com/__downloads/memory/ramdisk/Dataram_RAMDisk_4_4_0_RC31.msi</span></a><span style="font-family:宋体; font-size:10pt"><br /> </span>

<span style="font-family:宋体; font-size:10pt"><strong>一、创建虚拟内存盘<br /> </strong></span>

<span style="font-size:10pt">1、安装运行<span style="font-family:宋体">RamDisk 4G，如下图所示，例如创建一个1G（1024MB）容量的内存盘，FAT32磁盘格式、自动创建一个TEMP目录等设备。<br /> </span></span>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/060914_1547_Win7Win811.jpg) <span style="font-family:宋体; font-size:10pt"><br /> </span>

<span style="font-family:宋体; font-size:10pt">2、切换至Load/Save页面，自定义img映像目录，勾选开机自加载磁盘映像、关机时自动保存虚拟内存数据等设置。<br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/060914_1547_Win7Win812.jpg) <span style="font-family:宋体; font-size:10pt"><br /> </span>

<span style="font-family:宋体; font-size:10pt">3、然后点击&#8221;Start ramdisk&#8221;，安装磁盘驱动后，即可自动创建一个虚拟内存盘。<br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/060914_1547_Win7Win813.jpg) <span style="font-family:宋体; font-size:10pt"><br /> </span>

 

<p style="text-align: justify">
  <span style="font-family:宋体"><span style="font-size:10pt">二、<strong>迁移</strong></span><strong>系统变量</strong></span><span style="font-size:10pt"><br /> </span>
</p>

<span style="font-family:宋体">下面，我们需要更改下Win7、Win8.1系统设置，分别迁移用户变量和系统变量<span style="font-size:10pt">至RamDisk，</span>提升对日常临时文件的读取，设置如下：<br /> </span>

<span style="font-family:宋体">1、右击这台计算机，选择系统属性，依次<span style="font-size:10pt">选择&#8221;高级系统设置&#8221;-&#8220;高级&#8221;-&#8220;环境变量&#8221;；</span><br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/060914_1547_Win7Win814.jpg) <span style="font-family:宋体"><br /> </span>

<span style="font-family:宋体">2、分别<span style="font-size:10pt">修改</span>用户变量、系统变量中的<span style="font-size:10pt">Temp</span>、TMP路径值至<span style="font-size:10pt">Ramdisk</span>虚拟内存盘符，累计有四项修改，如下图所示。<br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/060914_1547_Win7Win815.jpg) <span style="font-family:宋体; font-size:10pt"><br /> </span>

<span style="font-family:宋体">为了方便用户手动恢复系统环境，阿象也整理Win7、Win8.1初始系统环境值，参考如下：<br /> </span>

<span style="font-family:宋体; font-size:10pt"><strong>用户变量：<br /> </strong></span>

<span style="font-family:宋体"><span style="font-size:10pt">TEMP：%USERPROFILE%\AppData\Local\Temp </span><br /> </span>

<span style="font-family:宋体; font-size:10pt">TMP：%USERPROFILE%\AppData\Local\Temp<br /> </span>

<span style="font-family:宋体; font-size:10pt"><strong>系统变量：<br /> </strong></span>

<span style="font-family:宋体; font-size:10pt">TEMP：%SystemRoot%\TEMP<br /> </span>

<span style="font-family:宋体; font-size:10pt">TMP：%SystemRoot%\TEMP<br /> </span>

<span style="font-family:宋体"><strong>三、迁移IE、火狐Firefox临时文件路径<br /> </strong></span>

<span style="font-family:宋体">通过<span style="font-size:10pt">修改浏览器临时</span>缓存<span style="font-size:10pt">路径，可以提高浏览器对临时文件的读取，修改后你会觉得浏览器的运行速度明显提高。</span><br /> </span>

<span style="font-family:宋体"><strong>1、设置IE10、IE11<span style="font-size:10pt">的Internet 临时文件夹路径</span></strong><br /> </span>

<span style="font-family:宋体"><span style="font-size:10pt">打开</span>IE浏览器<span style="font-size:10pt">，点击右上角的&#8221;工具&#8221;按钮，</span>依次<span style="font-size:10pt">进入&#8221;Internet选项&#8221;-&#8220;常规&#8221;-浏览器历史记录&#8221;设置&#8221;-点击&#8221;移动文件夹&#8221;，然后将路径改为到RamDisk</span>虚拟内存盘<span style="font-size:10pt">下即可。</span><br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/060914_1547_Win7Win816.jpg) <span style="font-family:宋体; font-size:10pt"><br /> </span>

<span style="font-family:宋体"><strong><span style="font-size:10pt">2</span>、设置火狐<span style="font-size:10pt">Firefox的临时</span>缓存<br /> </strong></span>

<span style="font-family:宋体"><span style="font-size:10pt">运行Firefox</span>火狐浏览器，<span style="font-size:10pt">在地址栏输入<strong>about:config</strong>，进入Firefox的配置页面；</span>然后在空白区域，<span style="font-size:10pt">右键点击Firefox配置界面新建字符串；</span><br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/060914_1547_Win7Win817.jpg) <span style="font-family:宋体; font-size:10pt"><br /> </span>

<span style="font-family:宋体">在新的字符串 值窗口中<span style="font-size:10pt">输入<strong>browser.cache.disk.parent_directory</strong></span>，点击确定；<span style="font-size:10pt">然后输入字符串的值</span>&#8220;<strong><span style="font-size:10pt">J:</span>\\<span style="font-size:10pt">TEMP</span>&#8220;</strong>，其中J代表当前的<span style="font-size:10pt">RamDisk</span>虚拟内存<span style="font-size:10pt">盘符即可。</span><br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/060914_1547_Win7Win818.jpg) <span style="font-family:宋体"><br /> </span>

<span style="font-family:宋体">最后<span style="font-size:10pt">重启FireFox</span>即可生效。<span style="font-size:10pt"><br /> </span></span>

<span style="font-family:宋体"><strong>四、<span style="font-size:10pt">修改Photoshop暂存盘路径</span></strong><br /> </span>

<span style="font-family:宋体">当我们用<span style="font-size:10pt">Photoshop</span>处理图片时，如果将PS<span style="font-size:10pt">暂存盘设置到RamDisk</span>虚拟内存盘<span style="font-size:10pt">上，可以大大提高Photoshop的</span>运行效率。<span style="font-size:10pt">一般地PS的缓存文件比较大，</span>因此建议设置较大的<span style="font-size:10pt">RamDisk</span>内存盘；如果没有大内存，阿象不建议<span style="font-size:10pt">修改Photoshop的暂存盘路径。<br /> </span></span>

<span style="font-family:宋体"><span style="font-size:10pt">具体操作如下：打开Photoshop，依次打开编辑-首选项-性能，更改你的暂存盘</span>位置，例如勾选J盘。<br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/060914_1547_Win7Win819.jpg) <span style="font-family:宋体; font-size:10pt"><br /> </span>

<span style="font-family:宋体"><strong>五、<span style="font-size:10pt">更改</span>迅雷、QQ旋风、IDM等<span style="font-size:10pt">软件下载</span>目录</strong><span style="font-size:10pt"><br /> </span></span>

<span style="font-family:宋体"><span style="font-size:10pt">如果</span>虚拟内存盘<span style="font-size:10pt">容量足够大，不妨将</span>第三方P2P软件的<span style="font-size:10pt">下载文件夹设置到RamDisk下，这样会大大减少下载对传统硬盘</span>或SSD固态硬盘<span style="font-size:10pt">的伤害。<br /> </span></span>

<span style="font-family:宋体"><strong>六、设置<span style="font-size:10pt">解压缩工具的临时解压文件的文件夹</span></strong><br /> </span>

<span style="font-family:宋体">例如<span style="font-size:10pt">WinRAR，打开WinRAR，点击菜单来的&#8221;选项&#8221;-&#8220;设置&#8221;，将默认的路径改至RamDisk</span>，<span style="font-size:10pt">如下图</span>所示。<br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/060914_1547_Win7Win8110.jpg) <span style="font-family:宋体; font-size:10pt"><br /> </span>

<span style="font-family:宋体">注意：<span style="font-size:10pt">有时候解压缩文件时产生的临时文件比较大，请确保你的RamDisk足够大。如勾选了了仅用于移动磁盘时，则只对移动盘的解压缩有效。<br /> </span></span>

<span style="font-family:宋体">以上只是介绍虚拟内存盘常用的方法，当然前提有大内存，才能提升Windows运行效率。如果你需要获得更快的体验，阿象建议你尽早使用SSD固态硬盘，拯救电脑硬盘的速度瓶颈。<br /> </span>

<span style="font-family:宋体; font-size:10pt"><br /> </span> 