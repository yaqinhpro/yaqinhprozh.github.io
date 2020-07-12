---
title: Mobile PsychicVR
date: 2016-09-15 17:44:50
tags:
---

**Time: Sep 2016 - April 2017**
**Advisor: PhD. Judith Amores and Prof.Pattie**
**Location: MIT Media Lab Fluid Interface Group**
**Type: Individual Research**

Mobile PsychichVR is the extension idea from PsychicVR, created by Judith Amores. It is an Andriod VR app that is integrated with MUSE brand sensing headband SDK. Cezar Cao finished the initial implementation and I am working on updating the app and putting more ideas into this app right now. 

\"We non-invasively monitor and record the electrical activity of the brain and incorporate this data in the VR experience using the MUSE headband. By sensing brain waves using a series of EEG sensors, the level of activity is fed back to the user via 3D content in the virtual environment. When the user is focused they are able to make changes in the 3D environment and control their powers. Our system increases mindfulness and helps achieve higher levels of concentration while entertaining the user.\" - quoted from Judith Amores.

Mobile PsychicVR shares the same vision but in a different platform. Currently, it supports single-player mode and multiplayer mode.

In single-player mode, you could control objects by using the brain power in Virtual Reality environment. 

In multiplayer mode,  you could interact with another user and use voice communication. We use Photon Realtime and Photon Voice to implement the connection and voice chat function.

<iframe src="//player.bilibili.com/player.html?aid=286044955&bvid=BV1Df4y1y7D4&cid=203900511&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" title="Mobile PsychicVR Single Player Demo Video"> </iframe>

First, open the app and open the Bluetooth in the phone. Then power the MUSE headband. Next step is clicking the \"Scan" button on the canvas and the available MUSE headband will be shown in the list. Next, click the \"Connect\" button. In both single-player MPVR and multiplayer MPVR, the debug interface is provided and will indicate the status of the connection. After successfully connecting the app and headband, in the debug interface, the waveform will display the real-time brain-wave data including the alpha, beta, gamma, theta, delta wave and EEG wave. The user could gaze \"Debug Mode\" to enable the debug interface or \"Disable Debug Mode\" to cancel the debug interface. Notice, all the buttons on the canvas could be gazed at except the \"Disconnect\" button, but it only could be clicked, which is to prevent accidently hit this button and cause disconnection.

In the single-player MPVR, the main functionality is to train the brain activity by using the VR world. The specific algorithm is used to detect the focus level of the user. If the user is focusing higher than some thresholds, he/she will have \"magic power\" in the VR world to control objects. If the user is focusing and gazing at some interactive objects, the object could be controlled by the user and visualized brain power will lift the targeted object.

In our 3.0 version app, we do not need an extra Android app anymore. All the functions are integrated in one Android app. So the user do not have to jump between different apps.

<iframe src="//player.bilibili.com/player.html?aid=201059794&bvid=BV1Xz411i74e&cid=203901655&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" title="Mobile PsychicVR Multi-Player Demo Video"> </iframe>

In the multiplayer MPVR, the main functionality is to visualize the mentality of the users and make the communication between users more interactive. The user will be represented by a spirit model in the VR world. The spirit model will change based on the user\'s brain activity. The main changes are: the body of the spirit will become more obvious if the user is more focused. The mental atmosphere will change color and size based on the brain activity. Also, the users could talk freely in the VR world. The users could quit the VR mode at any time and reenter again. This version supports maximum 2 users at the time.

<div align="center">
<img src="https://s1.ax1x.com/2020/06/20/NlW8k4.jpg" height="80px">
</div>

 


