
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
    - Normal mode - 30fps
    - Slow mode - Max fps supported by the camera

- Timelapse
    - 1080p
    - 1440p
    - 4k

  

## Usage

- Main button

    - Single press: Take picture or Start/End video

    - Double press: Change submode

- Right button

    - Long press: Connect to GoPro

    - Single press: Next mode

    - Double press: Previous mode

  

## Override uRequest lib
GoPro cameras HttpServer used for the WIFI API does not fully conform the HTTP protocol, because of that the uRequests library can not parse the response body. 
I have created a modified version of uRequests which works fine with GoPro WIFI API.

### How to
- Install the modified uRequests Micropython library

	-  [Download the library](https://github.com/jesuslg123/micropython-lib/blob/patch-1/urequests/urequests.py)

- Connect to your M5Stick device memory using the tool you prefer

	- Easy M5Stack [VS Code plugin](https://marketplace.visualstudio.com/items?itemName=curdeveryday.vscode-m5stack-mpy)

- Upload the urequests.py file into the "res" folder.

  

## TODO

- GoPro battery level

- Show current camera state

- Video duration

- Shoots & video time space on SD

- Settings view
