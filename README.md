# UESequencerSync

## Overview

This asset consists of an Unreal Editor Utility Widget and corresponding TouchDesigner component (.TOX file).

The Editor Utility Widget emits Unreal’s sequence editor current frame, start frame, end frame, framerate, and currently loaded sequence name via OSC. The .TOX enables TouchDesigner to receive this data and subsequently drives a designated time COMP so that it corresponds with Unreal’s sequencer.

[Here is a quick walkthrough video](https://www.dropbox.com/s/4jm60ywik976olw/UESequencerSync_Plugin.mp4?dl=0)

![Screenshot of UESequencerSync running in Unreal Engine and TouchDesigner.](https://images.squarespace-cdn.com/content/v1/5332dbfce4b0ba68c7397807/1648537262727-GGYM2MN7KSIG82K46R3L/UESequencerSync.png?format=1500w)

## Installation

Unreal Engine:
Copy UESequencerSync folder into `<YourProjectDirectory>/Plugins`.

TouchDesigner:
Use UESequencerSync.tox in your project and point to the desired time COMP. See TDSequencerSync.toe for example.
