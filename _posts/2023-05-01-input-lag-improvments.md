---
layout: post
title: "Input lag improvements"
date: 2023-05-01 11:31 -0300
---

This update focuses on improving input lag.

HaxBall now makes use of a canvas rendering feature that reduces rendering latency called [desynchronized canvas](https://developer.chrome.com/blog/desynchronized/). So far this feature is only implemented in chromium. This means it works in Chrome, Opera, Brave, Edge and any other chromium based browsers but doesn't do anything on firefox yet. This browser feature is relatively new so if you are using an old version of a browser there's a good chance it will not work.

The use of this feature is enabled by default but there's a new video setting called "Use low latency canvas" that can be used to disable it.

Additionally a small change to input handling was made. In previous versions HaxBall would process player input during the rendering phase. In this new version the input is processed directly in the html input event. This should save a few milliseconds of input lag. It is not as significant as the low latency canvas rendering but this improvement will work in all browsers.

**Changes:**
 * Implemented support for low latency canvas rendering.
 * Added "Use low latency canvas" setting to settings menu.
 * Improved player input handling latency.

As an added unintended bonus, it seems the low latency canvas fixes an issue where the latest version of chrome running with the `--disable-frame-rate-limit` option would freeze and crash. If you were running an old version of chrome in order to use this feature please give the latest chrome a try.

Edit: As of chrome 113 the desynchronized canvas doesn't fix the frame rate limit disabled issue. However there's a new fix, simply add --use-angle=d3d9 to the chrome command line. [Read more detailed instructions here](https://github.com/haxball/haxball-issues/wiki/Input-Lag#disable-frame-rate-limit).