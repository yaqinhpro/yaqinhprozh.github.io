---
title: HoloLens 1 Augmented Reality Streaming Solution
date: 2019-07-15 16:16:50
tags:
---

**Time: Dec 2018 - JUL 2019**
**Location: Dassault Systemes Solidworks Boston Campus eDrawings team**
**Role: Developer**

One most significant limitation of mobile devices including HoloLens is that the processing performance of the mobile devices is far behind the desktop devices.  That's where the idea of HoloLens streaming solution comes from. What if we could use the desktop device rendering power and also enjoy interacting with the AR devices? So we develope the streaming solution

<iframe src="//player.bilibili.com/player.html?aid=796012437&bvid=BV1iC4y1a7nw&cid=202549466&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" title="HoloLens 1 Augmented Reality CAD Model Viewer Demo Video"> </iframe>

A brief introduction for most of our components in our app:

## Load Model
User could open a Solidworks file just like eDrawings VR. Then user needs to run the Holographic Remoting Player app on Hololens and make sure the desktop and HoloLens are under same network. Click the AR button on eDrawings UI and enter the IP address of HoloLens, After the successful connection, user could see the streamed model from the desktop.

## Model Toolbar
The Model Toolbar includes five buttons: Explode, Scale, Rotate, Drag and Reset. The toolbar is in tag-along mode, which means it is always in the user's field of view. 

## Explode
Similar to the eDrawings explode feature, user could explode the model on HoloLens. Every component is moved at a certain distance in a certain direction from the center of the bounding box.  

## Scale
Loading a CAD model in real size is very important, so the app has the Scale feature. After the Scale button is pressed, the active model is scaled to one to one size. After the Scale button is depressed, the active model is scaled back to the table size.

## Rotate
In this mode, user could use the airtap and hold gesture to rotate the model. This app only allows horizontal rotation.

## Drag
In this mode, user could use the airtap and hold gesture to move the model. 

## Reset
The Reset feature resets the active model into the initial state.

<div align="center">
<img src="https://s1.ax1x.com/2020/06/19/NuTgbT.png" width="212px" height="40px"> <img src="https://s1.ax1x.com/2020/06/19/NuTRVU.png" width="125px" height="36px">    
</div>
