---
title: HoloLens 1 Augmented Reality CAD Model Viewer
date: 2018-12-15 21:55:40
tags:
---

**Time: May 2018 - Dec 2018**
**Location: Dassault Systemes Solidworks Boston Campus eDrawings team**
**Role: Main Developer**

In 2016, Microsoft released the first generation of HoloLens, HoloLens 1. More than traditional desktop devices, user could view the content in real 3D space. Compared to Virtual Reality devices, HoloLens could scan the physical environment and generate spatial data. The primary interaction method is the head movement, hand gesture, and also potentially controllers. Viewing the 3D CAD model in 3D space is definitely a powerful tool for CAD industry. So we start developing HoloLens 1 CAD model viewer app.

In this project, I work very closely with our Product Manager, Project Manager, Product Definition Engineer, User Experience Designer, and Quality Assurance Engineer in a team with Agile methodology to create this app.

<iframe src="//player.bilibili.com/player.html?aid=625883940&bvid=BV1Kt4y1y7cB&cid=198331202&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" title="HoloLens 1 Augmented Reality CAD Model Viewer Demo Video"> </iframe>

A brief introduction for most of our components in our app:

## LoadFile UI
Open the app, the first thing that shows up is the LoadFileMenu (in Follow Me mode). The app displays model buttons if this app is used before. If no sync is performed before, the menu is empty. The user could click the model button to load models. The LoadFileMenu could display at most 6 buttons on a page. If there is more than one page, Next page button and Prev page button shows up on the UI. Local/3DDrive button is to switch between syncing model files from HoloLens Local storage or 3DDrive cloud storage. The Prev/Next button is for going to the previous page or next page. The Settings button is used for launching the Settings menu. The Sync button is used for opening the Sync menu.

## Settings UI
​Settings Menu includes Hololens Local Storage target path and a switch to turn off/on the Mate Restriction Placement. By default, it’s on.

## Sync File UI
​User could use the Sync File UI to start syncing model files from HoloLens' local storage. After the Sync button is pressed, the app starts syncing files from HoloLens' local storage to app internal storage. The circle progress bar shows the syncing status. Once finished, the Sync File UI displays 'Sync Finished' so that user could go back to LoadFile UI to load models.

## Load Model
​After user airtaps one model button on the LoadFile UI, the app starts taking GLTF files and import the model. During the loading period, a loading box in Follow Me mode notifies user the model is still loading. User could cancel loading any time by pressing the Cancel button. After the model is loaded, it is in table size (so it is easy to control) and in follow me mode. Next, user could initialize the model by simply air taping it so the model exits follow me mode and the Model Toolbar is attached to its MRTK bounding box.

## MRTK Bounding Box
​This app uses the MRTK Bounding box for user-friendly manipulation. The MRTK Bounding box allows user to move, scale, rotate the model easily by using hand gestures without any restriction so that user could view the model in any size, from any position or from any angle. 

## Model Toolbar
​The Model Toolbar includes five buttons: Reset, Scale, Mate and Clear. As user moves, the model toolbar actively changes its position so it always faces the user. If the attached model is mated, it uses the stored mated date to determine its position, so it is not blocked by Spatial Mapping mesh. 

## Reset
The Reset feature resets the active model into the initial state. This includes resetting the active model back to table size, and back in Follow Me mode. This action also clears any stored mated data.

## Scale
​Viewing the CAD model in real size is very important, so the app has the Scale feature. After the Scale button is pressed, the active model is scaled to one to one size in two seconds. After the Scale button is depressed, the active model is scaled back to the table size. The process is animated. 

## Mate
​This app supports two mate modes.

The first one is Magnetic Mate for fast alignment. In Magnetic Mate mode, user could select one bounding box face of the active model and then the active model follows user's head gaze position with the selected bounding box face attached to the Spatial Mapping mesh. 

The second one is Shadow Mate for precise alignment w/o offset. By using our unique Shadow Mate tool, user could mate the active model to multiple surfaces with the target offset easily and efficiently.  In the Shadow Mate tool, when user looks at the distance rulers on the ruler part, a green slider appears and it includes text showing the precise distance from the Spatial Mapping mesh. User could either airtap the slider or the Mate button to place the active model

Mated bounding box faces are stored and used for the model to keep its alignment in other modes.  

## Clear
The Clear feature deletes the active model from the scene.

## Multiple Models
This app also supports handling multiple models. User could load and apply any feature into any model. 

<div align="center">
<img src="https://s1.ax1x.com/2020/06/19/NuTgbT.png" width="212px" height="40px"> <img src="https://s1.ax1x.com/2020/06/19/NuTRVU.png" width="125px" height="36px">    
</div>
