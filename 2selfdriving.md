---
layout: post
title: Self-Driving - Lane Detection
description: Program to detect lanes in a video
image: https://github.com/VipinindKumar/Self-Driving/raw/master/output/short1.0.gif
gif: https://github.com/VipinindKumar/Self-Driving/raw/master/output/out1.0.gif
nav-menu: true
show_tile: true
---

# Self-Driving - Lane Detection: program to detect lanes in a video 

## Version 1.0:

![1.0](https://github.com/VipinindKumar/Self-Driving/raw/master/output/out1.0.gif)

* Added smoothness of the average line between frames, to make the average line much more stable

## Version 0.9:

![0.9](https://github.com/VipinindKumar/Self-Driving/raw/master/output/out0.9.gif)

* Added a average of all the lines, as a single line in the video

## Version 0.85:

![0.85](https://github.com/VipinindKumar/Self-Driving/raw/master/output/out0.85.gif)

* Increase the quality of lines predicted by dilating the frame after canny function, which increases the width of the foreground objects making it easier to capture lines

## Version 0.8:

![0.8](https://github.com/VipinindKumar/Self-Driving/raw/master/output/out0.8.gif)

* Improve lines detection, using improved parameters values for HoughLInesP

## Version 0.5:

![0.5](https://github.com/VipinindKumar/Self-Driving/raw/master/output/out0.5.gif)

### Every frame from the video:
* is turned into grey-scale version using cv2.cvtColor function
* Finds edges in the frame using the [Canny86] algorithm by computing gradient, to identify change in pixels
* Using region_wants function discards the non-important areas of the frame for lane detection
* cv2.HoughLinesP to detect different lines passing through points detected by canny method
* Draw these lines on blank image of frame's size
* Use cv2.addWeighted function, to combine the original frame and empty image with drawn lines

[Github Repository - Self-Driving](https://github.com/VipinindKumar/Self-Driving)
