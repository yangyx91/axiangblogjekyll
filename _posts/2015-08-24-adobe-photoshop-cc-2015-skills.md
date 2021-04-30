---
id: 7662
title: 小技巧：Adobe Photoshop CC 2015吃内存、运行慢怎么弄？
date: 2015-08-24T21:18:06+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=7662
permalink: /adobe-photoshop-cc-2015-skills.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
smilie_vote_5:
  - "2"
views:
  - "14385"
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:7663;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_1:
  - "4"
categories:
  - Win10应用
  - 未分类
---
目前，行业权威应用软件Adobe Photoshop已经进入Adobe Photoshop CC 2015时代，全新适配Win10、3D打印等前沿技术，不过用户们发现这个版本很吃内存，经常运行速度慢，这是怎么回事？

笔者也参考网上大神的技巧，以Adobe Photoshop CC 2015(<a href="http://www.axiangblog.com/adobe-dreamweaver-cc-2015.html" target="_blank" rel="nofollow" >点击下载</a>)为例，借助Photoshop菜单里的“性能”选项，优化Photoshop的运行速度。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/08/photoshop-2015.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-7663" src="http://www.axiangblog.com/wp-content/uploads/2015/08/photoshop-2015.jpg" alt="photoshop-2015" width="450" height="265" /></a>  
首先打开“性能”选项，位置：“编辑”——>“首选项”——>“性能”

**内存使用状况**

适当增加Photoshop内存使用量可以增加软件运行效率，前提是电脑拥有足够内存容量，默认60-70%其实就很够用。当然很多电脑内存只是刚刚够用这样子，处理照片还会打开浏览器、聊天工具什么的，这时就要考虑压缩Photoshop内存用量，给其他软件预留空间。另外，如果平时Photoshop使用率不高，而且只是做一些简单处理，那么也可以适当压缩Photoshop内存用量。

**历史记录与高速缓存**

顾名思义，“历史记录”就是Photoshop里记录处理步骤的功能，默认记录步骤数量上限为50，如果用不到可减至20左右。在步骤记录左边的是“高速缓存级别和拼贴大小”，默认值4。如果你经常处理的文件比较大（100MB级别）、要用到很多图层，那么建议选择“文档较大”一项，反之则选择“文档较小”。一般来说，缓存级别越高，文件打开越慢，但打开后的处理速度就越快。

**图形处理器设置**

这里就是要动用显卡分摊部分显示、运算任务，要求用户必须拥有独立显卡，可以选择“使用图形处理器加速运算”和“使用OpenCL”选项。如果电脑没有显卡，则建议把所有选项里的勾去掉，不再耗费核显资源。

**暂存盘**

当内存用完的时候，硬盘将承载剩余的工作。默认暂存盘为系统盘，这会给本来就已经捉襟见肘的分区容量雪上加上。建议把暂存盘和系统盘分开，但是非系统版可能会导致性能下降，所以暂存盘最好还是选择固态硬盘。

当然，Photoshop还有其他优化设置要自行摸索和学习。