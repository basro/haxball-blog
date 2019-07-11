---
layout: post
title: 'Update: Custom team colors'
date: '2013-07-16T23:56:00-03:00'
tags: []
tumblr_url: https://blog.haxball.com/post/55661900492/update-custom-team-colors
---
<center><img alt="image" height="163" src="http://haxball.com/static/colors_ss.png" width="548"></center>
### Changes:

- Added a `/colors` chat command which lets room admins override the way in which the red and blue teams look.
- Added “Disable custom colors" to the options menu, enabling this makes the game ignore the custom team colors. (Useful if the admin has bad taste ;)

### /colors explained:

To set a team color you must have admin rights. Use it by typing the following command in the chat box:

`/colors <Team> <Angle> <AvatarColor> [Color1] [Color2] [Color3]`

**Team:** Should be either “red" or “blue", it specifies which team you are overriding.

**Angle:** Should be a number in the range 0…360. It specifies the angle in which the color stripes will be drawn.

**AvatarColor:** Should be RGB in hexa (ie: FF0000 for red), it specifies the color of the avatars.

**Color1, Color2, Color3:** Should be RGB in hexa (ie: FF0000 for red), they specify the colors of the team’s discs. The number of colors is optional, discs will have evenly sized stripes for each color specified.

And you can clear a team’s custom colors by using:

`/colors <Team> clear`

### Examples:

- 

White background with red avatar for red team:  
`/colors red 0 FF0000 FFFFFF`

- 

Red and white background with black avatar for red team in a 45 degree slope:  
`/colors red 45 000000 FFFFFF FF0000`

- 

Argentina’s flag colors for blue team:  
`/colors blue 90 FCBF49 75AADB FFFFFF 75AADB`

- 

Clear red team custom colors:  
`/colors red clear`

Enjoy!

