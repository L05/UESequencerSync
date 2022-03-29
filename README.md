# UESequencerSync

## Overview

This asset consists of an Unreal Editor Utility Widget and corresponding TouchDesigner component (.TOX file).

The Editor Utility Widget emits Unreal’s sequence editor current frame, start frame, end frame, framerate, and currently loaded sequence name via OSC. The .TOX enables TouchDesigner to receive this data and subsequently drives a designated time COMP so that it corresponds with Unreal’s sequencer.

This works for _in-editor_ workflows and deactivates when running PIE or stand alone so that any runtime sync logic can operate.

[Here is a quick walkthrough video](https://vimeo.com/693420311)

[![Screenshot of UESequencerSync running in Unreal Engine and TouchDesigner.](https://images.squarespace-cdn.com/content/v1/5332dbfce4b0ba68c7397807/1648574107752-0YTIB49A4RPSWSVF422C/UESequencerSync.png?format=1500w)](https://vimeo.com/693420311)

* 0:00 - Installation
* 2:08 - Unreal Setup
* 3:42 - TouchDesigner Setup
* 5:00 - Syncing Unreal and TouchDesigner
* 6:34 - Additional Notes

## Installation

### Unreal Engine
Copy UESequencerSync folder into `<YourProjectDirectory>/Plugins`.

### TouchDesigner
Use UESequencerSync.tox in your project and point to the desired time COMP. See TDSequencerSync.toe for example.
