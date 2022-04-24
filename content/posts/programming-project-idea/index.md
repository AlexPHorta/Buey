---
title: "I need a programming project idea"
slug: programming-project-idea
date: 2022-04-23T09:56:02-03:00
draft: false
tags:
- beginner
- programming
- projects
- ideas
---

![Bottom Up](bottomup.jpg)

The most common question I read in every thread, and I imagine you already have too, is "I'm new at programming and I want to practice, can someone give me some project ideas?".

Usually people have a very long list of responses right under the sleeve, and the options range from programming challenges to traditional and easy to build programs like a pomodoro timer, or a reminder. There are even complete projects devoted to this situation, some of them very interesting (and I'll list them at the end of this post), but I want to share a different approach.

Grab a simple app, like a hangman game, for example. Create the basic engine for the game, don't worry about the presentation. Simply choose a word and let the player guess it in a predefined number of chances. This basic engine will teach you about while loops, user input, and basic printing.

In a following iteration, you can add to the game a mechanism to retrieve words. Here, there are a couple of choices for implementation. It's possible to generate a list of words text file and retrieve a random line from it. That way you can learn about file manipulation, context managers, random access to files. Another solution is to use an API and retrieve the word from the web. There are many choices available, a simple search like random word api will present many options.

Next, a difficulty option. Now it's possible to create game modes with fewer number of choices, words with different number of letters, you can even research words that are most versus least common and separate the levels based on this characteristic. The inclusion of least common words can be made an option selected by the user and stored. These modifications can teach you the use of classes, more methods to access files, and the options can be stored in *ini*, *json* or *toml* files.

With the game engine ready, now it's time to think about the user interface. Here the choices abound. Pure text, a console framework like *ncurses* or *prompt_toolkit*, a desktop version, in *GTK*, *PyQT5*, or even *Tkinter*. A web version can be made with *Flask*, for example, and finally a mobile version with *Kivy*. Everything from a common code base. You can even develop every one of those versions, if you're careful enough, and that will teach you a lot.

All of this from a simple hanging man game. The same can be made with other basic apps, and each one of them will teach you other kinds of technologies. Threads, async code, REST, you name it. The gist of the technique is: don't be afraid of inserting features that don't make a lot of sense, or even of reinventing the wheel. The aim of the project is to help you learn programming concepts and not end up being a complete product.

To help you in picking up a project idea, I'll list some sources ahead, but not many of them, since I believe this method will help make the most of every single programming project you choose.

**[Project based ideas](https://github.com/practical-tutorials/project-based-learning): Tutorial based, and more complex project ideas, divided in different technologies and languages.**

**[App ideas](https://github.com/florinpop17/app-ideas): Those are divided by difficulty level, and come with complete use cases and possible improvements and tweaks that are close to the approach I lined up here. Excellent source.**
