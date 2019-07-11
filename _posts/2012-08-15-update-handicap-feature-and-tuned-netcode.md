---
layout: post
title: 'Update: Handicap feature and tuned netcode!'
date: '2012-08-15T00:05:00-03:00'
tags: []
tumblr_url: https://blog.haxball.com/post/29459206373/update-handicap-feature-and-tuned-netcode
---
This update is backwards compatible, so you won’t get any rooms marked with [OLD] this time, to check if you are running on this version try typing “/handicap” on the chat, it should print “\* Ping handicap requires a value in milliseconds”.

**Changes:**

- Added the /handicap chat command, it allows players to add lag to themselves while simultaneously reducing the lag with which other players will see their actions. Low ping players who are good sports can use this feature to level the playing field against more lagged players.
- The netcode has been improved a bit, the game should now be a bit more stable when the ping graph is noisy. It should also recover faster from a surge of lag spikes.
- Changed the ping display to better reflect the effective ping of the players, it will now show slightly higher ping than before if your ping is noisy.

**Handicap feature explained:&nbsp;**

You use this feature by entering “/handicap \<delay in milliseconds\>” into the chat. For example “/handicap 100” will add 100 milliseconds of ping to yourself. (Even the host can add lag to himself).

Every millisecond of lag you add to yourself will also reduce the lag/warp produced by your actions for every other player on the server by the same amount.

For example: Player A and player B are in a server. A has got 100msec of ping, B 200msec. If player A sets a handicap of 50msec to himself then he will have a total of 150msec of lag/warp, while at the same time player B will see player A’s actions with 50msec less lag/warp, which means he will see him with an effective 150msec of ping, thus A and B can now play in a more level field.&nbsp;

A good rule of thumb to achieve “lag fairness” is to set the handicap to half of the ping difference between you and the more lagged player you want to help out.

One very important thing to note is that by handicapping yourself you **will only reduce the lag/warp other players see of your own actions/movement** , it will not affect how much lag/warp other players see from anyone else’s actions/movement. **It is completely impossible to use this feature to gain any kind of advantage over other players** &nbsp;(unless you can convince them to voluntarily handicap themselves :P).

With this feature it is possible to play a 1v1 against someone across an ocean and still have it completely fair, instead of one player experiencing 300msec of lag and another player 0 it’s now possible to share the lag 50-50 as if you were playing in a host located exactly in the middle. You can also give yourself extra lag to balance against unskilled players ;)

Enjoy!

Edit: I found a bug and released a bugfix, read the next blog post for details.

