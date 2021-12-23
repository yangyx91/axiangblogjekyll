---
id: 3277
title: Windows Update更新速度太慢 自己动手集成Windows 8/8.1的安全更新补丁
date: 2013-09-30T01:46:22+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=3277
permalink: /windows-update-diy-windows-8-1.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "41421"
baidu_record:
  - "1"
smilie_vote_2:
  - "2"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:3276;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_3:
  - "3"
smilie_vote_4:
  - "2"
smilie_vote_6:
  - "2"
smilie_vote_1:
  - "3"
bigfa_ding:
  - "1"
love:
  - "2"
categories:
  - Win8.1
  - 未分类
---
<span style="font-size: 12pt;">本方法同样适用Win7系统<br /> </span>

<span style="font-size: 12pt;">现在很多人已经用上了Win8系统，但是在Win8在过去发布的一年内，微软累计为这款新系统提供了数十个的安全更新和功能更新，总计达到1G容量之多。如果每次安装好Win8后，要打齐这么多的补丁，真是费时费劲，如果遇到网络环境不佳或者微软服务器抽风，补丁打不齐全，又会让用户耿耿于怀。因此第三方的安全卫士一键打补丁功能很吃香，但是有些软件厂商将自家的产品冒充高危漏洞的补丁强行向用户提供，一时让Win8用户对这些&#8221;好意&#8221;的卫士或者管家产生顾虑。小编还是建议系统安全更新的事情交给最懂Windows的Windows Update组件，谢绝第三方参与。<br /> </span>

<span style="font-size: 12pt;">由于微软每个月都会发布新的安全更新，因此下载了Win8/Win 8.1的原始安装镜像也无法包含最新的安全补丁，当然Windows不退市，安全补丁是打不完的。何不自己手动将最新的安全更新或者功能更新一次性集成到安装镜像，这样不管是给他人安装还是自己重装都很方便，自从Win7开始，对于系统wim映像采用了DISM全新的系统部署工具，而我们就可以用DISM工具为自己的Win8/Win8.1系统集成各种更新补丁。<br /> </span>

&nbsp;

<span style="font-size: 14pt;"><strong>具体的操作步骤：<br /> </strong></span>

<span style="font-size: 12pt;"><strong>1、获取历史安全更新/功能更新补丁。<br /> </strong></span>

<span style="font-size: 12pt;">打开控制面板系统和安全，选择Windows 更新，查看更新历史记录<br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda1.png) <span style="font-size: 12pt;"><br /> </span>

<span style="font-size: 12pt;">然后记下已安装更新的编号，一般以KB开头，建议选择重要更新，对于可用重要更新，不建议集成。例如小编安装了Windows 8.1系统，只有一个安全更新KB2889543和一个功能更新KB2859675。<br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda2.png) <span style="font-size: 12pt;"><br /> </span>

&nbsp;

&nbsp;

<span style="font-size: 12pt;"><strong>2、下载这些安全更新的离线安装包。<br /> </strong></span>

<span style="font-size: 12pt;">首选的微软的下载中心（Microsoft Download Center）<br /> </span>

<span style="font-size: 12pt;">访问<a href="http://www.microsoft.com/zh-CN/download/default.aspx" target="_blank"  rel="nofollow" >http://www.microsoft.com/zh-CN/download/default.aspx</a> （输入更新编号查找，选择自己的系统版本，将补丁下载到本地备用。小编选择64位Win8.1系统版本下载离线安装包<br /> </span>

![](http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda3.png) <span style="font-size: 12pt;"><br /> </span>

&nbsp;

![](http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda4.png) <span style="font-size: 12pt;"><br /> </span>

&nbsp;

<span style="font-size: 12pt;"><strong>3、集成离线更新补丁到Win8/Win8.1系统镜像中<br /> </strong></span>

&nbsp;

<span style="font-size: 12pt;">例如：D盘新建一个Win8文件夹，分别新建wim文件夹（用于放置wim映像解压的系统文件）和updates文件夹（放置所以的离线更新补丁）<br /> </span>

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda5.png" /><span style="font-size: 12pt;"><br /> </span>
</p>

&nbsp;

<span style="font-size: 12pt;">加载Windows 8/8.1官方原始安装系统ISO镜像，复制镜像sources文件夹内的install.wim映像到D盘的win8文件夹内。<br /> </span>

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda6.png" /><span style="font-size: 12pt;"><br /> </span>
</p>

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda7.png" /><span style="font-size: 12pt;"><br /> </span>
</p>

<span style="font-size: 12pt;">使用DISM工具，Win+X，运行管理员身份的命令符，依次输入：<br /> </span>

<p style="text-align: center;">
  <p>
    <span style="font-size: 12pt;"><strong>dism /get-wiminfo /wimfile:d:\win8\install.wim</strong><br /> </span>
  </p>
  
  <p>
    <span style="font-size: 12pt;">//用于查询D盘win8文件夹内的wim映像的版本信息<br /> </span>
  </p>
  
  <p>
    &nbsp;
  </p>
  
  <p style="text-align: center;">
    <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda8.png" /><span style="font-size: 12pt;"><br /> </span>
  </p>
  
  <p style="text-align: center;">
    <p style="margin-left: 6pt;">
      <span style="font-size: 12pt;"><strong>dism /mount-wim /wimfile:d:\win8\install.wim /name:&#8221;Windows 8 Enterprise&#8221; /mountdir:d:\win8\wim</strong><br /> </span>
    </p>
    
    <p>
      <span style="font-size: 12pt;">//挂载wim映像中索引1企业版镜像到D:\win8\wim文件夹中。（你可以选择其它系统版本，比如Core、Pro版本）<br /> </span>
    </p>
    
    <p>
      &nbsp;
    </p>
    
    <p>
      <span style="font-size: 12pt;"><strong>dism /image:d:\win8\wim /add-package /packagepath:d:\win8\updates</strong><br /> </span>
    </p>
    
    <p>
      <span style="font-size: 12pt;">//将updates内的所有离线更新补丁批量添加到D:\win8\wim系统文件夹中<br /> </span>
    </p>
    
    <p style="text-align: center;">
      <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda9.png" /><span style="font-size: 12pt;"><br /> </span>
    </p>
    
    <p>
      <span style="font-size: 12pt;"><strong>dism /unmount-wim /mountdir:d:\win8\wim /commit<br /> </strong></span>
    </p>
    
    <p>
      <span style="font-size: 12pt;">//卸载已挂载的Windows 8.1企业版映像，并将D:\win8\wim内所有系统文件保存为install.wim映像。<br /> </span>
    </p>
    
    <p>
      &nbsp;
    </p>
    
    <p>
      <span style="font-size: 12pt;"><strong> 4、使用已经制作好的install.wim系统映像替换原始系统安装镜像内的install.wim映像，生成集成最新更新补丁的Windows8/8.1系统镜像。</strong><br /> </span>
    </p>
    
    <p style="text-align: center;">
      <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda10.png" /><span style="font-size: 12pt;"><br /> </span>
    </p>
    
    <p style="text-align: center;">
      <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/09/093013_0146_WindowsUpda11.png" /><span style="font-size: 12pt;"><br /> </span>
    </p>
    
    <p>
      <span style="font-size: 12pt;">至此，一款集成最新的安全更新/功能更新的Windows 8/8.1系统已经制作好，最后小编也建议该方法用于Win7或者Win8.1系统上，毕竟Win8是个过渡品。<br /> </span>
    </p>