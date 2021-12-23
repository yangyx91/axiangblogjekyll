---
id: 9816
title: 最新Win10开源UWP Community Toolkit v1.3社区工具包免费下载及使用上手
date: 2017-02-11T11:00:24+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=9816
permalink: /win10-uwp-community-toolkit.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "3770"
baidu_record:
  - "1"
categories:
  - Asp.Net
  - Web开发
  - Win10应用
  - 未分类
---
2017新年2月份 ，微软旗下全新开源UWP Community Toolkit社区工具包迎来v1.3重大版本更新，据官方称，新版可以为Win10 Build 10586平台开发UWP通用应用，运行在PC、Win10 Mobile、Xbox One以及Surface Hub、Hololens平台，有效简化了APP开发，整合了常用的helper函数、自定义控件以及app服务，支持使用C#或VB.NET编译，用于Win10全平台的生态圈的开发工作。

访问<a href="https://blogs.windows.com/buildingapps/2017/02/10/announcing-uwp-community-toolkit-1-3/" target="_blank"  rel="nofollow" >UWP Community Toolkit v1.3社区工具包官方博客</a>

<a href="http://www.axiangblog.com/win10-uwp-community-toolkit.html/uwp-community-toolkit1" rel="attachment wp-att-9817" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9817" src="http://www.axiangblog.com/wp-content/uploads/2016/08/UWP-community-toolkit1.jpg" alt="UWP-community-toolkit1" width="450" height="301" /></a>**UWP Community Toolkit v1.3社区工具包特色如下:**

1、Animations //动画特效

Blur(模糊)、Offset(偏移量)、Fade(淡入淡出)、Rotate(旋转)、Scale

2、Controls //控件

AdaptiveGridView //视图容器  
HamburgerMenu    //汉堡菜单  
HeaderedTextBlock//标题文本  
ImageEx          //相册  
PullToRefreshListView//下拉即刷新效果  
RadialGauge          //发散性度量  
RangeSelector        //范围选择器  
RotatorTile          //旋转体标题  
SlideableListItem    //滑动列表成员

2017.2更新

WrapPanel //

TextboxMask和TextBoxRegex (attached properties)//输入框控件

SurfaceDialTextboxHelper (attached property)//新控件

MarkdownTextBlock//

TileControl//标题控件

ScrollHeader//滑动头部

Expander//

AdvancedCollectionView//高级集合视图

Loading control//加载控件

3、Code Helpers//Helper函数

Colors、Connection、Converters、ImageCache、StorageFiles、Streams、VisualTreeExtensions、WeakEventListener

4、Services//服务支持

Bing、Facebook、Twitter、新增OneDrive服务、微软翻译服务

5、Notifications//通知中心

Tiles       //动态磁贴  
Toasts      //任务栏的“吐司”通知

6、**Animations动画**

Light//加亮

Reorder grid animations (attached property)

ParallaxService//视觉服务

7、可用性

8、模板APP集成

**UWP Community Toolkit v1.3社区工具包上手使用：**

1、下载安装Visual Studio 2015（含Update3）中文版（<a href="http://www.axiangblog.com/visual-studio-2015-update3.html" target="_blank"  rel="nofollow" >点击下载</a>）、Windows 10 RS1 SDK离线包（<a href="http://www.axiangblog.com/win10-anniversary-sdk-win10-mobile.html" target="_blank"  rel="nofollow" >点击下载</a>）

参考资源：《<a href="http://docs.uwpcommunitytoolkit.com/en/master/" target="_blank"  rel="nofollow" >http://docs.uwpcommunitytoolkit.com/en/master/</a><a href="http://www.axiangblog.com/docs-microsoft-com-uwp-win10.html" target="_blank"  rel="nofollow" >》</a>

2、打开VS2015，创建或者打开一个空白Universal Windows project(UWP项目) 解决方案

<a href="http://www.axiangblog.com/win10-uwp-community-toolkit.html/uwp-community-toolkit2" rel="attachment wp-att-9818" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9818" src="http://www.axiangblog.com/wp-content/uploads/2016/08/UWP-community-toolkit2.jpg" alt="UWP-community-toolkit2" width="500" height="347" /></a>3、在Visual C#模板下创建一个通用UWP空白应用

4、向该项目中添加UWP Community Toolkit v1.0社区工具包

<a href="http://www.axiangblog.com/win10-uwp-community-toolkit.html/uwp-community-toolkit3" rel="attachment wp-att-9819" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9819" src="http://www.axiangblog.com/wp-content/uploads/2016/08/UWP-community-toolkit3.jpg" alt="UWP-community-toolkit3" width="400" height="387" /></a>5、在解决方案资源管理器面板中，右击自己的项目名，选择&#8221;管理NuGet包&#8221;

<a href="http://www.axiangblog.com/win10-uwp-community-toolkit.html/uwp-community-toolkit4" rel="attachment wp-att-9820" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9820" src="http://www.axiangblog.com/wp-content/uploads/2016/08/UWP-community-toolkit4.jpg" alt="UWP-community-toolkit4" width="450" height="316" /></a>6、在线搜索&#8221;Microsoft.Toolkit.UWP&#8221;、依次选择所需的软件包进行安装

**小提示：NuGet程序包**

Microsoft.Toolkit.Uwp  
//主NuGet包，包含专用颜色的Helper代码、网络连接检测、存储文件处理和流的Helper类

Microsoft.Toolkit.Uwp.Notifications  
//通知中心包-可以用代码生成Win10 UWP动态磁贴、Toast通知以及badge徽章通知

Microsoft.Toolkit.Uwp.Notifications.Javascript  
//通知中心包-JavaScript包。

Microsoft.Toolkit.Uwp.Services  
//网络服务包-包括Bing、Facebook和Twitter服务helper函数。

Microsoft.Toolkit.Uwp.UI  
//用户界面UI包-包含XAML代码转换器、可视化树状图扩展以及XAML UI的helper函数。

Microsoft.Toolkit.Uwp.UI.Animations  
//动画和组件行为包，包括模糊、淡入淡出、旋转等效果。

Microsoft.Toolkit.Uwp.UI.Controls  
//XAML控件，支持RadialGauge、RangeSelector等效果。

7、在项目的XAML或C#代码页面添加对UWP Community Toolkit v1.0的引用

a.在XAML页面的头部，添加引用页面

**<Page  x:Class=&#8221;MainPage&#8221; xmlns:controls=&#8221;using:Microsoft.Toolkit.Uwp.UI.Controls&#8221;**

b.在C#页面的命名空间之前，using导入官方的工具箱

**using Microsoft.Toolkit.Uwp;**  
**namespace MyApp**  
**{**

**现在下载更多UWP Community Toolkit v1.3社区工具包的模板、文档以及代码**，<a href="https://github.com/Microsoft/UWPCommunityToolkit" target="_blank"  rel="nofollow" >https://github.com/Microsoft/UWPCommunityToolkit</a>

当然微软也准备了一款《UWP Community Toolkit Sample App》应用（<a href="https://www.microsoft.com/en-us/store/p/uwp-community-toolkit-sample-app/9nblggh4tlcq" target="_blank"  rel="nofollow" >Win10商店下载</a>），可以直接查看各类控件的源码。