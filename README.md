## Go M5tick Pro Remote controller

A GoPro Remote Control implementation using UIFlow for StickC of StackM product, based on ESP32 board.

![GoPro Remote using StickC](https://github.com/jesuslg123/gopro-remote-stickC/blob/master/StickC_Remote.png)

## Features
#### Camera mode change
- Photo
	- No timer
	- 3 seconds timer
	- 10 seconds timer
- Video
- Timelapse

## Usage
- Main button
	- Single press: Take picture or Start/End video
	- Double press: Change submode
- Right button
	- Long press: Connect to GoPro
	- Single press: Next mode
	- Double press: Previous mode


## TODO
- Autoconect to GoPro on startup
- Document how to override uRequests library
- GoPro battery level
- Show current camera state
	- Video duration
	- Shoots & video time space on SD
- Settings view

