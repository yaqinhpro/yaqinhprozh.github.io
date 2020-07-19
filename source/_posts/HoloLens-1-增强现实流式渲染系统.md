---
title: HoloLens 1增强现实流式渲染系统
date: 2019-07-15 16:16:50
tags:
---

**时间： 2018年12月 - 2019年7月**
**地点： Dassault Systemes Solidworks波士顿地区eDrawings团队**
**职责： 开发人员**

移动设备最大的限制之一是远远落后于桌面设备的处理性能。基于这个原因，我们研发了HoloLens流式渲染系统。如果我们能用桌面设备的渲染能力的同时也尽情享受增强现实设备的交互呢？所以我们研发了流式渲染系统。

<iframe src="//player.bilibili.com/player.html?aid=796012437&bvid=BV1iC4y1a7nw&cid=202549466&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" title="HoloLens 1 Augmented Reality CAD Model Viewer Demo Video"> </iframe>

下面是关于APP大部分组件的简短介绍：

## 加载模型
就像eDrawings虚拟现实程序一样，用户能够加载Solidworks文件。然后用户需要在HoloLens上启动全息远程播放器APP，确保电脑和HoloLens在同一个网络下。在eDrwaings桌面版本中点击进入增强现实按钮，然后输入HoloLens的IP地址。在连接成功后，用户能够从eDrwaings桌面版本传输模型数据。

## 模型工具栏
模型工具栏包含了5个按钮：爆炸图，放大缩小，旋转，移动，重置。工具栏处于跟随模式中，这样工具栏就能经常保持在用户的视野中。

## 爆炸图
和eDrawings爆炸图模式相似，用户能够在HoloLens上爆炸图模型。以包围盒中心为参考，每一个部件都沿着特定的方向移动了特定的距离。

## 放大缩小
能够查看真实大小下的CAD模型的能力很重要，所以我们打造了放大缩小模式。在按下放大缩小按钮之后，模型会设定成真实的大小。在取消放大缩小按钮之后，模型会设定回桌面大小。

## 旋转
用户能够使用点击手势来旋转模型。APP只允许水平旋转。

## 移动
用户能够使用点击手势来移动模型。

## 重置
重置功能会将模型设置回最初的状态。

<div align="center">
<img src="https://s1.ax1x.com/2020/06/19/NuTgbT.png" width="212px" height="40px"> <img src="https://s1.ax1x.com/2020/06/19/NuTRVU.png" width="125px" height="36px">    
</div>
