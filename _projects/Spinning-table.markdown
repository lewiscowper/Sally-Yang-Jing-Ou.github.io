---
layout: project
date: 2014-09-19
title: Spinning Table (iOS Game)
languages: Swift
summary: to learn Swift and SpriteKit
thumbnail: /img/projects/Spinning-Table/thumb.jpg
screenshots: 
 - ["/img/projects/Spinning-Table/Screenshot1.png", "/img/projects/Spinning-Table/1thumb.jpg", ""]
 - ["/img/projects/Spinning-Table/Screenshot2.png", "/img/projects/Spinning-Table/2thumb.jpg", ""]
 - ["/img/projects/Spinning-Table/Screenshot3.png", "/img/projects/Spinning-Table/3thumb.jpg", ""]
 - ["/img/projects/Spinning-Table/Screenshot4.png", "/img/projects/Spinning-Table/4thumb.jpg", "Game Over"]
 - ["/img/projects/Spinning-Table/Screenshot5.png", "/img/projects/Spinning-Table/5thumb.jpg", "Score can be shared on social media"]
---

This simple game was created for the purpose of getting familiar with Swift and SpriteKit. You may view the code [here](https://github.com/Sally-Yang-Jing-Ou/SpinningTable).
<br> I have used Double Dispatch for collisions detections (instead of hard coding it like I did in the last game I made).

Frameworks/Tools Used:
---
Language:
<li>Swift</li>

Frameworks:
<li>SpriteKit</li>
<li>UIKit</li>
<li>Foundation</li>

General Rules:
---
<li>Each time the screen is touched, the Player will jump to the inner loop</li>
<li>Eating a Star gains you two points</li>
<li>Eating a Heart gains you one point as well as a Life</li>
<li>Touching a Shuriken leads you to Game Over, or decreases your Life count (if you have more than 0 Life)</li>
<li>Running out of the map also leads you to Game Over</li>
<li>Level increases as you gain more points, the speed at which the Players move/spin will increase as well </li>
<li>You may click Replay or Share the results on social media</li>

Known Issues:
---
If you're using Xcode6 Beta3:

When you first run the game, you might (or might not) encounter an error that says: "thread 1:EXC_BREAKPOINT (code=EXC_i386_BPT, subcode=0x0)". The solution to this is to do Product -> Clean

If you're using Xcode6 Beta4:

"'CGFloat' is not convertible to 'NSTimeInterval'" is an error that might occur, a temporary solution is to cast the variable into "Double", at the lines that are failing
<br>The path created using SKShapeNode does not show up (this issue doesn't occur in Beta3). Good to know that I am not the only one that's seeing this issue: http://stackoverflow.com/questions/24951185/in-xcode-6-beta-4-stroking-with-skshapenode-doesnt-work-anymore & https://devforums.apple.com/message/1011007#1011007
<br>No good solutions have been found for the above issues, yet.

Update:
----
Code has now been updated to match the changes made to the lastest Xcode, it should now be running on iOS8 (Xcode6 Beta7) simulator. 