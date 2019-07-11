---
layout: post
title: 'Update: Custom stadiums and HaxBall anniversary!'
date: '2011-12-05T21:32:00-03:00'
tags: []
tumblr_url: https://blog.haxball.com/post/13808360727/update-custom-stadiums-and-haxball-anniversary
---
Time sure flies! It has already been 1 year since HaxBall was first released and ever since the game has never stopped growing in popularity. Last Friday was an all time record of 100k unique visitors in a single day!

It has been a while since the last update and for that I apologize. Some of you might have heard that I was working on a dedicated server for HaxBall, this was an Adobe Air version which would let you host rooms without the overhead of graphics, sounds and running on a browser. Unfortunately the performance during testing was a bit underwhelming so this project has been postponed for now.

Today I bring to you a new and exciting feature: The HaxBall Stadium Format (.hbs). This is a text format which allows you to create any kind of stadium! From boring things like just changing the size of the goal to crazy shaped stadiums with multiple goal areas and obstacles.

The .hbs files are plain text so you can edit them with any text editor.

Here are two sample stadiums:

- [simplestadium.hbs](http://www.haxball.com/stadiums/simplestadium.hbs)
- [simplestadium\_tutorial.hbs](http://www.haxball.com/stadiums/simplestadium_tutorial.hbs) (Same as simplestadium but it contains comments which should help you understand the format. If you plan to create HaxBall stadiums this one is a must read.)
- [funkystadium.hbs](http://www.haxball.com/stadiums/funkystadium.hbs)

For now there is no documentation, if you want to learn to make stadiums you’ll have to figure it all out by tinkering with these sample stadiums. I’ll make a stadium format reference page in the future though.

I have one warning: The stadium format is in alpha stage and will definitely be changing. There’s a good chance that stadiums made for the current version of this format will stop working on upcoming updates, although they will be easy to fix/update.

In future versions of this format I’ll add the possibility of changing physical parameters of the players and balls (radius, kick strength, friction, speed, mass, etc.). I also plan to add features that will let you create things like speed boosters, bumpers, teleporters, high friction ground, etc. I’m really excited to see what kind of things the community will do with this :)

**Changes:**

- &nbsp;Changed the UI to pick stadiums, there’s now a “Pick” button which will open a stadium select popup.
- Added a new default map called “Huge” for 4v4 5v5 and above. (Dimensions are subject to further tuning).
- Implemented the HaxBall Stadium Format (.hbs). You can load .hbs files from your hard drive by pressing the “Load” in the new stadium picker UI.
- Fixed a bug which made the score limit, time limit and stadium buttons visible even when a game was in progress.

Enjoy!

