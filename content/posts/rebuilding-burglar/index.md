---
title: "Rebuilding Burglar"
date: 2023-03-21T21:17:20
draft: false
slug: rebuilding-burglar
---

I had the idea of making Burglar sometime in 2018.  It would be a *match-3* style game, but with a twist.  The stones wouldn't follow a rectangular grid, but a circular one.  In a way, it's something like four binary trees arranged in a circle.  The stones appear randomly in one of the four central slots.  Then, you have to decide if you move the grid clockwise or counter-clockwise.  Choice made, the stone will migrate to the immediate outer circle in the direction of your choosing, and another one will surge in the center (in one of the four central slots and of random color).  When the stone reach the outermost circle, it stops there.  You can remove stones of the same color by aligning at least three of them in one of the circles.  When there are no more available slots, the game ends. It's pretty funny (at least for me), when played in the basic level, and really hard when played in the more advanced ones.

For the very first version of the game I used a Python framework named [Pilas](https://www.pilas-engine.com.ar/).  I liked this one framework a lot, but couldn't manage to pass the initial phases of development.  I believe it was my fault, and I'm really curious to know how this framework evolved.

After some more research, I decided to use [Pygame](https://www.pygame.org/).  It was a good choice, only blemished by my complete lack of experience building games.  Don't get me wrong, I could manage to make a working prototype of the game, but it was really far from usable by the end user, because I didn't know how to effectively program the animations.  The stones simply jump from one slot to the other, with no visual indication of the dance the stones were making.  It makes the game a bit confusing in the final stages, when you have a lot of stones and nowhere to make some disappear.

Below you can see a video I made of the game playing.  It gives you the general idea of the concept.

{{< youtube id="CwcwrPgyltA" title="Burglar Game Playing">}}

<s>Well, since I really like the concept I decided to remake Burglar, but now using a Javascript framework (Phaser).  This will allow the program to be played in web browsers and other devices.  Only this time I'll properly learn the framework before attempting to rebuild the software.</s>

Update: No, I'll improve the code in the Python version first. Then, I'll properly learn Javascript, then the framework, and then rebuild the game. First things first!

In case you liked the game, you can download it at the [repository](https://codeberg.org/Buey/Burglar).  If you know Javascript stuff, your help is more than welcome. Drop me a line so we can get this ball rolling!
