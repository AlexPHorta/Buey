.. title: I need a programming project idea.
.. slug: programming_project_idea
.. date: 2020-03-19 14:54:30 UTC-03:00
.. tags: programming, project idea, python
.. category: programming
.. link:
.. description:
.. type: text

.. image:: /images/bottomup.jpg
    :alt: I need a programming project idea.

`Laced together against a windy sky`_ by sagesolar_ is licensed under `CC BY-ND 2.0`_.
    .. _`Laced together against a windy sky`: https://www.flickr.com/photos/sagesolar/33580319133/in/photolist-TanUXx-yAB61d-2ipRrQ8-HzGE4R-2euU9yz-HGMW66-NbiiR1-2hcv7og-refy1q-Ctap96-2d2opTr-7ggfPB-263gR2w-2hwoAAL-2hBdMY8-2hKu28m-2go3Bt7-mrfjFy-dgE5nL-2hyZaZD-23X71eA-7kZjvW-2iaNCje-2hXAKhp-XXUSvG-YkdZxz-23HxejP-2hvx1ov-2h33cUk-zWfZbR-sfrUH6-231PvcD-2gBpQR4-2gy14qi-6nZKRt-2gjeJrP-27Zp6pQ-2a2y4Jh-QfuPv5-2cBGjSx-LdCCAg-37YPf-23eraWF-2gFcGV3-2c7rTYx-mrdv9c-sYMRWC-s791Nn-51xSkA-E21RyR
    .. _sagesolar: https://www.flickr.com/photos/sagesolar/
    .. _`CC BY-ND 2.0`: https://creativecommons.org/licenses/by/2.0/

The most common question I read in every thread, and I imagine you already have too, is "I'm new at programming and I want to practice, can someone give me some project ideas?".

Usually people have a very long list of responses right under the sleeve, and the options range from programming challenges to traditional and easy to build programs like a pomodoro timer, or a reminder. There are even complete projects devoted to this situation, some of them very interesting (and I'll list them at the end of this post), but I want to share a different approach.

Grab a simple app, like a hangman game, for example. Create the basic engine for the game, don't worry about the presentation. Simply choose a word and let the player guess it in a predefined number of chances. This basic engine will teach you about while loops, user input, and basic printing.

In a following iteration, you can add to the game a mechanism to retrieve words. Here, there are a couple of choices for implementation. It's possible to generate a list of words text file and retrieve a random line from it. That way you can learn about file manipulation, context managers, random access to files. Another solution is to use an API and retrieve the word from the web. There are many choices available, a simple search like *random word api* will present many options.

Next, a difficulty option. Now it's possible to create game modes with fewer number of choices, words with different number of letters, you can even research words that are most versus least common and separate the levels based on this characteristic. The inclusion of least common words can be made an option selected by the user and stored. These modifications can teach you the use of classes, more methods to access files, and the options can be stored in *ini*, *json* or *toml* files.

With the game engine ready, now it's time to think about the user interface. Here the choices abound. Pure text, a console framework like ncurses or prompt_toolkit, a desktop version, in GTK, PyQT5, or even Tkinter. A web version can be made with Flask, for example, and finally a mobile version with Kivy. Everything from a common code base. You can even develop every one of those versions, if you're careful enough, and that will teach you a lot.

All of this from a simple hanging man game. The same can be made with other basic apps, and each one of them will teach you other kinds of technologies. Threads, async code, REST, you name it. The gist of the technique is: don't be afraid of inserting features that don't make a lot of sense, or even of reinventing the wheel. The aim of the project is to help you learn programming concepts and not end up being a complete product.

To help you in picking up a project idea, I'll list some sources ahead, but not many of them, since I believe this method will help make the most of every single programming project you choose.

`Project based ideas`_: Tutorial based, and more complex project ideas, divided in different technologies and languages.
    .. _`Project based ideas`: https://github.com/tuvtran/project-based-learning

`App ideas`_: These are divided by difficulty level, and come with complete use cases and possible improvements and tweaks that are close to the approach I lined up here. Excellent source.
    .. _`App ideas`: https://github.com/florinpop17/app-ideas
