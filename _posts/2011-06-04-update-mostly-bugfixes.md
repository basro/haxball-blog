---
layout: post
title: 'Update: Mostly bugfixes.'
date: '2011-06-04T01:36:49-03:00'
tags:
- udpate
tumblr_url: https://blog.haxball.com/post/6167555471/update-mostly-bugfixes
---
 **Changes:**

- Improved location detection, this update will reduce the number of users who get an incorrect flag.
- Optimized the room list, it will load faster. The latest Flash Player update (version 10.3) seemed to change something that made my old room list implementation freeze for several seconds when loading the rooms, this update should fix that.
- Fixed a bug which cause player nicknames and avatars to move and scroll wildly if they were prefixed with a tab character.
- Fixed a bug that made the suggested replay names have incorrect month numbers. 
- Added the string “HBRP” in ASCII encoding to the replay file format right after the version number ( bytes 4 to 7 ). This is here to help sites that host HaxBall replay files identify them.
- Added the chat command “/clear\_avatar”, which will remove whatever avatar you have set.

Not the most exciting update ever, but enjoy it anyway! ;)

