---
id: 2227
title: Win7忘记登录密码怎么办？不慌，两句命令就能搞定
date: 2013-02-22T02:01:36+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=2227
permalink: /win7-password-forget.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "6691"
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:2226;s:11:"_thumb_type";s:10:"attachment";}'
categories:
  - Win8.1
  - 未分类
---
首先声明：本次教程只适用于学习测试，增加电脑操作技能，由于涉及系统用户安全性，请勿用于非法用途

&nbsp;

从2009年以来，win7的市场占有率一直高涨，大有第二个xp系统的美称。。。。说实话，无论是用户体验，还是软件兼容性，还是新特色功能，这些，xp系统是远远不能比的，阿象还是建议坚守xp阵营的童鞋们，是时候该升级系统了。

安装一款新的操作系统后，由于都是个人PC，很多人第一步骤是给自己的win7系统加个登录密码，安全性和隐私性大大得到提升。。。。**说实话，阿象个人没这个习惯，担心忘记密码。。。。。下面还真说中了。**

于是，时间长了，电脑如果闲置久了，网站注册用户以及其他各种账号，密码。。。。终于，有一天，我的win7用户登录密码，forgotten，忘记了。。。。。着急啊，电脑桌面还有机密文件啊，总不能重装系统吧，**不慌，两句命令就能搞定。  
** 

**教程原理解析：就是调用系统自带组件，就是cmd命令符，重新新建，加入administrator级别的标准管理员，其权限远远高于用户个人新建的普通管理员账户，就这样，借用一个高级账户，重新登陆win7系统，及时找回原先C ：\用户，目录下原先的用户，通过复制，找回原先桌面上的资料，文件，即可。。。。最后，再次新建的普通用户管理员账户，至于密码，那就随便了。。。。。别忘记了，新建管理员后，系统自带的administrator级别的标准管理员也需要禁用掉，以防被黑，被破解。。。  
** 

工具：需要一个U盘，一个win7 PE镜像。。。。提前制作好支持U盘启动的win PE

步骤：（以下是个人模拟测试教程）**系统：windows Thin PC**，一款精简版的win7旗舰版系统，适合测试，学习体验。虚拟机：Vmware workstation 9

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win71.jpg" />
</p>

1、首先要有一个**普通用户管理员账户，例如&#8221;阿象&#8221;，也加个密码&#8221;axiangblog.com&#8221;  
** 

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win72.jpg" />
</p>

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win73.jpg" />
</p>

2、创建用户后，重启，这时win7登陆界面如下：

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win74.jpg" />
</p>

3、提示输入密码，如果密码错误，就会出错

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win75.jpg" />
</p>

4、输入正确密码，登陆后，**系统自带的administrator级别的标准管理员也需要禁用掉，**才能重新模拟测试用户现实环境。

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win76.jpg" />
</p>

某天，阿象个人密码忘记，无法登陆win7，那就需要教程的支持了。

<ol style="margin-left: 40pt;">
  <li>
    <div>
      插入U盘，开机U盘启动win PE，不限制是32位还是64位，内核在6.1以上。
    </div>
    
    <p style="text-align: center;">
      <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win77.jpg" />
    </p>
  </li>
  
  <li>
    到系统目录：C:\windows\system32下，找到系统组件magnify.exe（即，屏幕放大镜）
  </li>
</ol>

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win78.jpg" />
</p>

3、更改magnify.exe和cmd.exe两个系统组件**所有者为administrators**，然后更改**所有权限为&#8212;完全控制**。（如下图操作）

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win79.jpg" />
</p>

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win710.jpg" />
</p>

4、重命名&#8212;-Magnify.exe改为Magnify.exe1，cmd.exe改为magnify.exe（也是为了后面直接调用cmd命令符做准备）

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win711.jpg" />
</p>

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win712.jpg" />
</p>

5、更改后，重启电脑，（U盘要拔掉）登陆原先的win7系统

6、点击左下角的轻松访问，启用放大镜&#8212;&#8211;（也通过前面PE的修改，顺利调用出cmd命令符，）

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win713.jpg" />
</p>

7、键入：

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win714.jpg" />
</p>

net user administrator /active:yes /表示新建系统administrator标准管理员

net user administrator &#8220;&#8221; /表示重置密码，密码为空

8、关闭命令符窗口，重启（右下角图标）

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win715.jpg" />
</p>

9、然后win7登陆界面，如下。。增加了administrator账户。。离成功不远了

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win716.jpg" />
</p>

10、点击administrator，顺利进入系统。。。。。。。。至此，win7系统登陆已经被突破了，毕竟权限更高一级。

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win717.jpg" />
</p>

11、Magnify.exe1， magnify.exe先后还原

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win718.jpg" />
</p>

12、**原来的&#8221;阿象&#8221;账户，即使有密码的保护**，还是可以删除。。。

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win719.jpg" />
</p>

13、最终，还是删除了。

<p style="text-align: center;">
  <img alt="" src="http://www.axiangblog.com/wp-content/uploads/2013/02/022213_0201_Win720.jpg" />
</p>

至此，win7的账户登录已经完全突破，原理简单，两句命令就解决了。。。。。但是简单的背后，**阿象个人感觉win7的登录存在不安全性，如果电脑里面有重要资料，就这样就可以轻易登录系统，窃取资料。。。。。。个人建议，重要资料还是要加密，或者放在外置的移动存储设备里面，毕竟电脑只是一个学习，工作的工具，而不是个人隐私保险柜。。。更不是你的日记本，阿象通过这个测试，告诫大家，资料不要放在一个篮子里面，不要以为一个用户账号加个密码，就可以安枕无忧了。。。。安全防范之心不可无。  
** 

&nbsp;

**幸好，win8引入了本地账户以及微软账户双重账户的机制，其中微软账户的安全性更高，完全基于云的理念，更大限度保护用户的安全性，而且将电脑OS视为一个软件、工具。。。。。如果有系统安全恐惧症的童鞋，也可以升级到win8系统。。。。。  
** 

**  
**