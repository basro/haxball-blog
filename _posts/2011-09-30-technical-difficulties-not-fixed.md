---
layout: post
title: Technical Difficulties (not fixed)
date: '2011-09-30T14:48:00-03:00'
tags: []
tumblr_url: https://blog.haxball.com/post/10854646576/technical-difficulties-not-fixed
---
The server is having some troubles and I’m trying to figure out what has gone wrong. Please have patience until this is fixed.

**Update:**

At last, it’s fixed! For those curious and linux savvy, the cause was that /dev/random was not replenishing fast enough, causing the server threads to block waiting for random numbers.

For the record, this has been the longest downtime in HaxBall’s history: About 6 hours.

It has also been the most stressful 6 hours of this year :)

**Update:**

As some of you may have noticed HaxBall has gone down again twice this week, I apologize for it. I thought I had fixed the problem last friday but it keeps happening. I still think the cause is entropy depletion though.

If there’s any linux sysadmin gurus who would like to give me a hand I’d gladly accept it :)

**Update:**

Ok, so I was probably chasing a wrong lead with that /dev/random bullshit :P, the server just happened to go back up the time I tried out something related to it last time.

Anyway, I’ve now changed another server setting which I believe could be a definite fix, but I’ll wait a few days before claiming victory. This didn’t work either.

