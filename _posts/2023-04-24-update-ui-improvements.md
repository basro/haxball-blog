---
layout: post
title: "UI Update and some bugfixes"
date: 2023-04-24 11:00 -0300
---
This update focuses on improving the utilization of the screen's real estate. It should be specially useful for anyone playing on a small screen.

**Changes:**
 * The chat box is now resizable by dragging from the top.
 * The chat box will expand when the chat text field is focused. (Height configurable from video settings)
 * The chat box is now translucent. (Opacity configurable from video settings)
 * The game viewport will now occupy the whole screen.
 * The game viewport will continue to render even when accessing the room's lobby menu.
 * The site's nav bar will now disappear when you join a room, freeing up 35 pixels for the actual game.
 * Removed the chat box send button.
 * Removed 'restricted' view mode option. This was an artifact of the move from flash to html5, I don't believe anyone was using it.
 * Pressing number 4 will now select 1.75x Zoom instead of the now removed 'restricted' view mode.
 * Nicer scrollbars in the room's teams lists.
 * Fixed bug where the game camera would stop working permanently until leaving the room after witnessing the game physics going awry.
 * Fixed bug where some browsers would be wrongly detected as not supporting datachannels.
