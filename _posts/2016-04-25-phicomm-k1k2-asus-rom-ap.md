---
id: 9402
title: Phicomm斐讯K1/K2无线路由器如何刷华硕固件、设置中继AP无线模式
date: 2016-04-25T22:15:26+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=9402
permalink: /phicomm-k1k2-asus-rom-ap.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "21760"
baidu_record:
  - "1"
smilie_vote_2:
  - "5"
smilie_vote_3:
  - "1"
smilie_vote_4:
  - "1"
smilie_vote_5:
  - "1"
love:
  - "2"
categories:
  - Win10应用
  - 未分类
---
上月底，笔者分享了Phicomm斐讯公司中K1、K2两款免费1200M无线路由器，其中官方固件可以一键开启拨号上网、Wifi无线中继等功能，但对于高级玩家来说，希望路由器可以加入更多的网络服务功能，比如今天分享下K1玩家热衷的华硕固件，不容错过。

喜欢原版官方固件，可以参考《<a href="http://www.axiangblog.com/phicomm-k1k2-v21-4-4-8.html" target="_blank"  rel="nofollow" >Phicomm斐讯K1/K2无线路由器官方固件v21.4.4.8上手使用篇 附下载</a>》

<a href="http://www.axiangblog.com/phicomm-k1k2-asus-rom-ap.html/breed-web7" rel="attachment wp-att-9409" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9409" src="http://www.axiangblog.com/wp-content/uploads/2016/04/breed-web7.jpg" alt="breed-web7" width="450" height="320" /></a>  
随着技术的发展，升级路由器ROM也是非常方便，玩家可以直接在路由器后台操作，即可完成升级工作。

下面，笔者为大家分享下Phicomm斐讯K1/K2无线路由器如何刷华硕固件操作流程，参考如下：

1、用网线连接Win10 PC电脑、Phicomm斐讯K1路由器，访问路由器后台，例如http://192.168.1.1/（具体以cmd的ipconfig查看路由器网关为准）

<p style="text-align: left;">
  <a href="http://www.axiangblog.com/phicomm-k1k2-asus-rom-ap.html/breed-web8" rel="attachment wp-att-9410" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9410" src="http://www.axiangblog.com/wp-content/uploads/2016/04/breed-web8.jpg" alt="breed-web8" width="360" height="336" /></a><br /> 2、对Phicomm斐讯K1路由器官方固件降级到v1.0.0.3，玩家需要在系统管理的升级中，手动上传SW_K1_703004393_V1.0.0.3.bin（<a href="http://pan.baidu.com/s/1bMuqdw" target="_blank"  rel="nofollow" >见网盘</a>），路由器将重启完成降级工作。
</p>

3、下载大神们打造的“路由器刷breed Web助手通用版（支持k1全自动）”小助手，<a href="http://qiannao.com/ls/huzibbs/01399c29" target="_blank"  rel="nofollow" >更新地址</a>

<p style="text-align: left;">
  <a href="http://www.axiangblog.com/phicomm-k1k2-asus-rom-ap.html/breed-web1" rel="attachment wp-att-9403" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9403" src="http://www.axiangblog.com/wp-content/uploads/2016/04/breed-web1.jpg" alt="breed-web1" width="450" height="285" /></a><br /> 解压后，以管理员身份，右击运行“路由器刷breed web控制台通用版.exe”主程序，保持默认配置，开始刷Breed，等待路由器2分钟后，拔掉电源；
</p>

4、按住路由器重置键，再次接通Phicomm斐讯K1路由器电源，等待几秒后松开重置键，继续访问路由器后台，例如http://192.168.1.1/（具体以cmd的ipconfig查看路由器网关为准），这时将自动进入“Breed Web恢复控制台”；

<p style="text-align: left;">
  <a href="http://www.axiangblog.com/phicomm-k1k2-asus-rom-ap.html/breed-web2" rel="attachment wp-att-9404" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9404" src="http://www.axiangblog.com/wp-content/uploads/2016/04/breed-web2.jpg" alt="breed-web2" width="450" height="191" /></a><br /> 这里可以查看Phicomm斐讯K1路由器官方硬件配置，基本上是入门级别。
</p>

CPU     MediaTek MT7620A ver 2, eco 6  
内存     64MB DDR2  
Flash     Winbond W25Q64 @ 24MHz (8MB)  
以太网     MediaTek MT7620A built-in 5-port 10/100M switch  
时钟频率     CPU: 580MHz, Bus: 193MHz  
编译日期     2016-04-19 [git-3b445d3]  
版本     1.0 (r849)

5、最后，我们在系统更新中，上传华硕固件RT-AC54U-GPIO-1-PSG1208-64M_3.4.3.9-099.trx（<a href="http://pan.baidu.com/s/1bMuqdw" target="_blank"  rel="nofollow" >免费下载</a>），完成彻底的路由器刷机工作。

<p style="text-align: left;">
  <a href="http://www.axiangblog.com/phicomm-k1k2-asus-rom-ap.html/breed-web6" rel="attachment wp-att-9408" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9408" src="http://www.axiangblog.com/wp-content/uploads/2016/04/breed-web6.jpg" alt="breed-web6" width="450" height="217" /></a><br /> 6、现在，我们可以体验华硕ASUS专业的路由器后台，体验比如VPN、SS、广告过滤、迅雷快鸟、中继AP无线模式，不容错过。
</p>

笔者以华硕固件设置中继AP无线模式为例，比如2.4Ghz无线工作模式选择最后一项“ap clinent+ap”；

<p style="text-align: left;">
  <a href="http://www.axiangblog.com/phicomm-k1k2-asus-rom-ap.html/breed-web4" rel="attachment wp-att-9406" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9406" src="http://www.axiangblog.com/wp-content/uploads/2016/04/breed-web4.jpg" alt="breed-web4" width="430" height="377" /></a><br /> 无线AP-Client角色可选“Lan Bridge有线桥接”或者“Wan无线模式”，在STA SSID搜索附近的基地台，选择对应的主路由器MAC地址和名称，输入密钥，即可。
</p>

<p style="text-align: left;">
  <a href="http://www.axiangblog.com/phicomm-k1k2-asus-rom-ap.html/breed-web5" rel="attachment wp-att-9407" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9407" src="http://www.axiangblog.com/wp-content/uploads/2016/04/breed-web5.jpg" alt="breed-web5" width="400" height="353" /></a>
</p>

<p style="text-align: left;">
  终于，我们可以愉快上网了！
</p>