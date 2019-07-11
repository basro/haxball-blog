---
layout: post
title: Latest Chrome update breaks HaxBall.
date: '2012-08-07T15:51:00-03:00'
tags: []
tumblr_url: https://blog.haxball.com/post/28925836001/latest-chrome-update-breaks-haxball
---
Chrome has recently released an automatic update which changes the flash player it uses. This new flash player (called Pepper Flash) seems to have issues with HaxBall and may cause lag and all sort of other problems.

If you are experiencing problems playing HaxBall in Chrome I highly recommend you try with another browser like [Firefox](http://www.mozilla.org/en-US/firefox/new/ "Firefox site") or [Opera](http://www.opera.com/ "Opera site").&nbsp;

Meanwhile I’ll be trying to find a way to make HaxBall work properly in Pepper Flash.

Please help spread the word.

**Update:**

After doing some tests, it seems like the hardware acceleration mode might be the cause of some of the issues &nbsp;(For those who know flash this option sets wmode = direct in the embed script). Interestingly enough disabling hardware acceleration doesn’t seem to decrease the rendering performance with Pepper Flash, so in the next update I’ll make that feature be ignored if Pepper Flash is detected.

I still recommend using another browser (or disabling Pepper Flash player) since it seems pepper flash is a bit more cpu intensive than the vanilla flash player, but hopefully this change will improve the situation for Chrome users.

