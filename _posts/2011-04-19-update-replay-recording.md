---
layout: post
title: 'Update: Replay recording!'
date: '2011-04-19T21:59:19-03:00'
tags:
- updates
tumblr_url: https://blog.haxball.com/post/4764698694/update-replay-recording
---
At last, I’m done with replays! This feature has certainly taken more time and effort to complete than what I initially thought it would. For those curious, some form of per-room player ban is next on the list.

**Changes:**

- Added a rec button, press it once to start recording, press it again to stop and save the recorded gameplay as a .hbr file!
- Added a “Replays” button to the room list, use this to load previously saved replays.
- Added a ping graph option, enabling it will display a graph of your ping history (Doesn’t show if you are the host).
- Added a new URL parameter which lets users link to replay files. [Try it!](http://www.haxball.com/?replay=0#http://www.haxball.com/demo.hbr "Click here to try it out!") Detailed explanation below.

**Replay links explained (gets a bit technical):**

A replay link has the following format:

“http://www.haxball.com/?replay=_\<Replay Version\>_#_\<Replay URL\>”_

\<Replay Version\> is currently 0, but this number will change every time a new version of HaxBall is released. HaxBall replay files (.hbr) have got this number stored in their first 4 bytes (as a big-endian unsigned integer), which should be useful if someone wanted to implement some sort of HaxBallReplay-Tube (wink wink ;).

\<Replay URL\> is the URL of the .hbr file to load.

Example: [http://www.haxball.com/?replay=0#http://www.haxball.com/demo.hbr](http://www.haxball.com/?replay=0#http://www.haxball.com/demo.hbr)

There’s also a small catch, because of Flash security policies your file host needs have a [crossdomain.xml policy file](http://active.tutsplus.com/tutorials/tools-tips/quick-tip-a-guide-to-cross-domain-policy-files/ "crossdomain.xml policy file") allowing haxball.com (and haxball.appspot.com) to read files from it.

