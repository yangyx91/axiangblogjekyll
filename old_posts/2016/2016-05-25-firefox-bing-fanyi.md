---
id: 9562
title: 火狐Firefox老玩法：申请微软免费云翻译+全文调用必应翻译服务？
date: 2016-05-25T22:51:12+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=9562
permalink: /firefox-bing-fanyi.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "7007"
baidu_record:
  - "1"
categories:
  - Win10应用
  - 未分类
---
喜爱科技、游戏的玩家常会去看国外网站，但面对外文更是压力山大，于是有了谷歌一键翻译、有道机器翻译等工具，不过如果你是一个微软、火狐Firefox爱好者，那可以结合微软翻译Azure网络云服务，开启火狐Firefox浏览器的翻译工具栏，一键翻译各类外文网站。

<a href="http://www.axiangblog.com/firefox-bing-fanyi.html/firefox-translate4" rel="attachment wp-att-9566" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9566" src="http://www.axiangblog.com/wp-content/uploads/2016/05/firefox-translate4.jpg" alt="firefox-translate4" width="450" height="347" /></a>  
笔者也参考网上的教程，整理了如何申请微软必应翻译服务、调用火狐Firefox浏览器翻译工具栏，具体参考如下：

1、访问微软“Microsoft Translator”服务，<a href="https://datamarket.azure.com/dataset/1899a118-d202-492c-aa16-ba21c33c06cb" target="_blank"  rel="nofollow" >点击这里</a>

ps：区域切换成美国，网页语言可选中文简体，登陆个人的微软账号，注册2,000,000字符/月免费版，即可。

<a href="http://www.axiangblog.com/firefox-bing-fanyi.html/firefox-translate1" rel="attachment wp-att-9563" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9563" src="http://www.axiangblog.com/wp-content/uploads/2016/05/firefox-translate1.jpg" alt="firefox-translate1" width="500" height="169" /></a>  
2、申请翻译服务成功后，我们还需单独创建一个App程序，<a href="https://datamarket.azure.com/developer/applications/save" target="_blank"  rel="nofollow" >点击创建</a>；

<a href="http://www.axiangblog.com/firefox-bing-fanyi.html/firefox-translate2" rel="attachment wp-att-9564" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9564" src="http://www.axiangblog.com/wp-content/uploads/2016/05/firefox-translate2.jpg" alt="firefox-translate2" width="450" height="318" /></a>  
例如创建“阿象的在线翻译”，可设定重定向URI/描述项，最后将生成一个App客户端ID、客户端密钥。

3、下载安装一个火狐Firefox浏览器，参考《<a href="http://www.axiangblog.com/firefox-46.html" target="_blank"  rel="nofollow" >改进JavaScript安全性 火狐Firefox46中文版官方下载</a>》

4、配置Firefox浏览器，接入微软必应翻译网络服务；

<a href="http://www.axiangblog.com/firefox-bing-fanyi.html/firefox-translate3" rel="attachment wp-att-9565" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9565" src="http://www.axiangblog.com/wp-content/uploads/2016/05/firefox-translate3.jpg" alt="firefox-translate3" width="400" height="259" /></a>  
打开 **about:config**  
修改“**browser.translation.ui.show**”的值为“true”  
修改“**browser.translation.detectLanguage**”的值为“true”  
新建字符串“**browser.translation.bing.clientIdOverride**”设定值为“客户端ID”，比如axiangblog  
新建字符串“**browser.translation.bing.apiKeyOverride**”设定值为“客户端密钥”，比如mwC4n95npJVqmxuonmEXO5s0aZUdcAt1OzSG8fkrEQs=

<a href="http://www.axiangblog.com/firefox-bing-fanyi.html/firefox-translate5" rel="attachment wp-att-9567" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9567" src="http://www.axiangblog.com/wp-content/uploads/2016/05/firefox-translate5.jpg" alt="firefox-translate5" width="450" height="216" /></a>  
5、重启火狐Firefox浏览器，完成配置，访问各类外文网站，即可开始全文翻译服务。