---
id: 4944
title: 火狐技巧：如何解决Firefox、Flash假死问题，附解决方案
date: 2014-06-22T11:21:07+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=4944
permalink: /firefox-adobe-flash.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "6965"
cover:
  - ""
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:4943;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_6:
  - "1"
categories:
  - Win10应用
  - 未分类
---
说到常用浏览器，不得不提到火狐狸。不知不觉中，火狐浏览器从最早的Firefox3.0直接跨入Firefox30历史。从Firefox29开始，火狐自动将Flash插件加入点击播放白名单。这也意味着用户访问网页时，火狐将自动加载Flash内容。

但是在日常使用中，不少童鞋打开过多Flash网页时，常常遇到Flash假死，直接导致火狐浏览器停止响应，尤其在机械硬盘上更为严重。

本着不断探索，发现问题的精神，阿象也为忠实的火狐用户整理浏览器技巧，如何彻底解决Firefox、Flash假死问题。

**方案一、设置&#8221;点击播放&#8221;  
** 

由于火狐Firefox默认将Flash网络播放器加入白名单，因此每次访问网页后，火狐都将自动加载Flash，因此瞬时占用大量的系统资源。因此，我们可以给火狐加入&#8221;点击播放&#8221;功能。这次依旧感谢勤劳的开发者，我们只需一款FlashBlock扩展，即可为加入点击播放功能。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062214_1121_Firefo1.jpg) 

**FlashBlock扩展下载**：<a href="https://addons.mozilla.org/zh-cn/firefox/addon/flashblock/" target="_blank"  rel="nofollow" >https://addons.mozilla.org/zh-cn/firefox/addon/flashblock/</a>

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062214_1121_Firefo2.jpg) 

&nbsp;

**方案二、去除Flash沙箱、屏蔽Flash P2P上传  
** 

从Flash 11.3开始，Adobe引入保护模式（Protected Mode），即Flash沙箱功能。虽然可以保护用户免受恶意网站感染，但这项沙箱机制常常导致页面假死等问题。

另外，火狐等主流浏览器均支持识别恶意网址，进一步提升网络安全性，因此，我们完全可以去除Flash沙箱保护模式。

**具体操作如下**：（适用Win7、Win8、Win8.1平台）

1、安装最新Flash for Firefox正式版：

<a href="http://download.macromedia.com/pub/flashplayer/current/support/install_flash_player.exe" target="_blank"  rel="nofollow" >http://download.macromedia.com/pub/flashplayer/current/support/install_flash_player.exe</a>

2、访问系统盘，修改 mms.cfg，其文件所在位置如下：

Windows 32位: C:\windows\system32\macromed\flash

Windows 64位: C:\windows\syswow64\macromed\flash

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062214_1121_Firefo3.jpg) 

3、复制mms.cfg至非系统盘，然后用记事本打开编辑，手动添加

ProtectedMode=0

RTMFPP2PDisable=1

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062214_1121_Firefo4.jpg) 

4、最后将新mms.cfg直接替换旧文件，即可

**方案三、切换IE内核  
** 

这是比较个性DIY的方案，兼具两者各自的优缺点，虽然火狐版Flash容易导致崩溃，但Win8.1内置Flash插件非常稳定，很少出现问题。

因此，我们可以给火狐用上IE内核，随时切换访问大量Flash网页，轻松组成双核，例如大家熟悉的&#8221;解雇IE&#8221;扩展，兼容最新版火狐浏览器。

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062214_1121_Firefo5.jpg) 

**解雇IE扩展下载**：<a href="https://addons.mozilla.org/zh-CN/firefox/addon/fire-ie/" target="_blank"  rel="nofollow" >https://addons.mozilla.org/zh-CN/firefox/addon/fire-ie/</a>

**方案四、换个浏览器  
** 

如果你是普通上网用户，又不喜欢折腾的话，就换个浏览器，例如IE。。。。。。。。。

**阿象结语：  
** 

如果你也是爱好学习、折腾的技术青年，相信你不会被Flash假死等问题屈服，只要自己努力尝试，最后还是能找到解决方法的。