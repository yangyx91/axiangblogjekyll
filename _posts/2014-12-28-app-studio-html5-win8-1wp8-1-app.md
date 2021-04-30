---
id: 6401
title: 如何用微软APP Studio为HTML5网站开发Win8.1/WP8.1通用应用？
date: 2014-12-28T22:00:12+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=6401
permalink: /app-studio-html5-win8-1wp8-1-app.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "9846"
baidu_record:
  - "1"
bigfa_ding:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:6399;s:11:"_thumb_type";s:10:"attachment";}'
categories:
  - Asp.Net
  - Web开发
  - Win10应用
  - 未分类
---
本月中旬，微软对自家免费在线应用开发平台Windows App Studio进行功能更新，首次新增TouchDevelop和Web App Template两项重磅特性。借助这两项新特性，开发爱好者可以快速将一个HTML5网站、网页游戏、博客、论坛程序原生移植为一款APP应用或游戏。 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio1.jpg) 

注： 

1、TouchDevelop是一个全新的Windows Phone软件开发环境，是第一个可以使用手机编程的应用，包括一个物理引擎和用户界面框架组合形式。 

2、通用Web App Template（WAT——Web应用模板），原生支持Win8.1、WP8.1通用应用方案。 

下面，阿象就带各位Win8.1、WP8.1爱好者快速学习下如何将一个Web网站或游戏移植为一款APP应用程序。 

操作步骤： 

1、访问Windows App Studio：http://appstudio.windows.com/ 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio2.jpg) 

2、登陆自己的微软账户，选择&#8221;开始新的项目&#8221;，默认模板参考如下。这次，我们只需选择Web App Template模板。 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio3.jpg) 

3、接下来的流程具体分为四步骤：填充内容、选择主题、设置磁贴和应用介绍。（注意：点击右上角Save可实时保存当前的存档和数据） 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio4.jpg) 

例如你有博客，这时首先填写&#8221;APP title（应用名称）&#8221;（可更改应用ICON图标，推荐PNG格式图片），然后在Base Url中填写网址，左侧也可以实时预览应用界面。 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio5.jpg) 

随后我们可以对应用内的APPBar按钮和功能更改，例如将英文替换为中文，或者修改图标和操作动作。 

4、下面就是选一套应用主题，比如暗黑色、明亮色，也可以自定义。 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio6.jpg) 

5、在磁贴栏目，我们可以分别设置磁贴类型（旋转式、循环式、图标式风格，阿象推荐第三种风格）、APP启动时界面设置。 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio7.jpg) 

在图标式磁贴风格中，我们可以设置340x340px icon图标、应用名称、应用简要（最多三行）；在启动界面栏目下，需分别设置WP8.1启动界面和锁屏界面、win8.1启动界面截图。 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio8.jpg) 

6、最后一步就是填写应用简介、应用语种、应用隐私策略（Win8.1应用若需联网使用，就默认需加上开发者个人的隐私策略说明的网页地址）。 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio9.jpg) 

如果你有开发者账号，可以直接绑定开发者ID，APP ID等信息。 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio10.jpg) 

该隐私策略需以网页完整的形式进行展示说明，证明该Win8.1或WP8.1应用遵从微软应用开发政策隐私保护规则，不会获取普通用户的个人数据。 

![](http://www.axiangblog.com/wp-content/uploads/2014/12/122814_1401_APPStudio11.jpg) 

7、完成以上所有工作后，我们只需点击Finish，然后Generate，即可直接生成一款Win8.1/WP8.1通用应用的本地安装包、源代码（默认为C#和.Net编译）。 

注：阿象之前已向微软MSDN反馈尽快将HTML5+JS语言加入到Windows App Studio编译语种中，希望尽快可以实现。 

后面我们就可以直接用VS 2013、VS 2015对源代码编译或配置，也可以本地部署、截图应用快照、关联微软开发者账号、生成Windows Store应用上传专用包，最终在商店上架。