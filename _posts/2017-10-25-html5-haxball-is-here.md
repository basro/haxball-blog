---
layout: post
title: HTML5 HaxBall is here!
date: '2017-10-25T07:43:55-03:00'
tags: []
tumblr_url: https://blog.haxball.com/post/166777593021/html5-haxball-is-here
---
Give it a try [html5.haxball.com](http://html5.haxball.com)

Found something wrong with it? Dont panic! This is an alpha version, it’s bound to have bugs and lack features. My top priority is reaching feature parity with the flash version and new features may come after that. If you find a bug please report it [here](https://github.com/haxball/haxball-issues/issues).

The flash version and html5 versions will coexist until feature parity is reached.

## Screen/Viewport size

One notable difference with flash version of haxball is the bigger use of the screen. This is something I always wanted to do, but since flash was not hardware accelerated it wasn’t possible to do it at a reasonable framerate.

However, a bigger viewport can make the game look really tiny (specially if your screen is 1080p or above). For this reason I’ve added camera-zoom feature. You can change between 3 different zoom levels using number keys 1 to 3.

Some people have expressed to me that they would rather have the restricted viewport size that the flash version had, this is something I’m considering as an option. If this matters to you too let me know.

## Netplay

The netplay works very similarly to the flash version but uses WebRTC instead of RTMFP.

If you have issues connecting to room hosts but were able to do it in the flash version you should report it [here](https://github.com/haxball/haxball-issues/issues).

You will notice ping will be a bit lower than usual, this is mainly because in flash network events were handled 60 frames per second while in html5 the events are handled immediately and independent of the screen refresh rate. This meant that flash could add about 32msec of latency depending on how close to the frame updates the network packets would arrive.

Another nice improvement is that the game will no longer lag if the host changes tabs. (flash would lower it’s frame rate and thus handle network events even less frequently)

