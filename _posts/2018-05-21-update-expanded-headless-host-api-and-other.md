---
layout: post
title: 'Update: Expanded Headless Host API and other things.'
date: '2018-05-21T12:49:49-03:00'
tags: []
tumblr_url: https://blog.haxball.com/post/174117632521/update-expanded-headless-host-api-and-other
---
The Headless Host API has been expanded, check the full changelog [here](https://github.com/haxball/haxball-issues/wiki/Headless-Host-Changelog).

Also a few small changes to the haxball client:

### Changes:

- Fixed bugged /handicap feature. (This was only working correctly if you were the room host, now it should work for clients too.)
- Added chat log notifications for when a player is given admin rights.
- Very minor improvements to netcode.

### What I’ll be working on next:

I’ve spotted a small bug in the netcode which is basically disabling a fairly significant optimization I had made. Unfortunately fixing this bug seemed to cause new bugs to pop up elsewhere that actually break the game and not just make it less optimal.

So until next update, I’ll be focusing on getting these bugs fixed.

