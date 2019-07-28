---
layout: post
title: Update!
---

This update is pretty big and involved some considerable internal restructuring, I'd not be surprized if I broke some custom stadiums in the process. Please report if you notice anything has broken.

**Game changes:**

 * Implemented a video setting for disabling custom avatars.
 * Improved the order in which players will appear in the chat autocompletion list.
 * Implemented a ball kicking ratelimit option which lets you configure how often players can kick the ball. This might be useful to level the playing field between people who are using key repeat macros and players that simply use their fingers. This can be accessed with the /kick_ratelimit chat command (which only admin players can use)
 * Added a lot of new physics features. Among them gravity vectors, a new physics object called "Joint" which can join two discs together, the ability to make any disc kickable or scorable (including players), a configurable kickback force and more. [Here's a video showing gravity and joints](https://youtu.be/H-SAUrE0RwY)
 * Changed the maximum value of extrapolation to 50ms. This feature has been quite a controversial feature and while I don't believe it gives players any advantage it was also never meant to be used with values higher than this anyway.

**Headless Host Changes:**

You can read full changelog [here](https://github.com/haxball/haxball-issues/wiki/Headless-Host-Changelog).

 * Added the ability to remove the headless host player from the player list.
 * Added room announcements with configurable styling and sounds.
 * Added the ability to get and modify all properties of any disc in the game.
 * Added the ability to override the avatar of a player.
 * Added a convinient way to reorder the list of players.
 * Added the ability to set the new ball kicking rate limit options.

 **Stadium (.hbs) File Changes:**

 There's a lot of changes, the full changelog is [here](https://github.com/haxball/haxball-issues/wiki/Stadium-(.hbs)-File-Changelog).

 The stadium files documentation has been revamped and completed, you can read it [here](https://github.com/haxball/haxball-issues/wiki/Stadium-(.hbs)-File).