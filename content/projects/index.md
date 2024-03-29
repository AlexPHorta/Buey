
---
title: "Projects"
date: 2023-03-16T09:20:26-03:00
draft: false
featured_image: '/images/gohugo-default-sample-hero-image.jpg'
---

NSEW Virtual Keyboard
===========================

NSEW is a virtual keyboard designed for text insertion with the directional keys of a remote controller (up, right, down, left and enter) or a numpad.  The normal keyboard layout (a retangular box) is clumsy when used with this kind of device or in these specific conditions.

NSEW solves this situation minimizing the number of strokes needed to select a specific character, in accordance with the common letter frequency of the selected language (English is the default).

{{< youtube id="hl489lGkHnE" title="NSEW Virtual Keyboard in action." >}}

The user presses the directional keys until the desired character is under the cursor, then presses ENTER (or 5, in this demonstration).  The chosen character is inserted in the field area and the cursor gets back to the central position (the Mode key).

The NSEW Virtual Keyboard was developed in plain Javascript, and I intend to make it a real package some time soon (for now it's legacy code, until I figure out how to use one of Javascript's test frameworks).  Any help with the development is welcome, just drop me a line, or open a PR.

[Live preview.](https://www.buey.net.br/nsew/ "NSEW Virtual Keyboard live preview")

[Repository of the project.](https://codeberg.org/Buey/NSEW-Keyboard/ "NSEW Virtual Keyboard on Codeberg")

Burglar
=========

Burglar is a *match-3* game I created some time ago. It's somewhat peculiar because it uses a circular grid for the stones, instead of a retangular one. Unfortunately, it's still not finished, and probably will never be (at least this version). Created with Pygame. Ah, and it's legacy software, alright? When (if) I rewrite it I'll properly test it.

{{< youtube id="CwcwrPgyltA" title="Burglar Game Playing">}}

[Repository of the project.](https://codeberg.org/Buey/Burglar)

Numex
======

Get written numbers (and money quantities) from numbers.  In Brazilian Portuguese.  This one I would really love to have enabled in my work (I have to write large money quantities from time to time).

Numex was written in Python. If you have any ideas for improving this package, drop me a line or open a PR.

Usage
------

Basic numbers:

```
>>> import numex
>>> numex.numeroPorExtenso(2398764)
>>> 'dois milhões, trezentos e noventa e oito mil, setecentos e sessenta e quatro'
```

Money quantities (brazilian Real):

```
>>> import dindin
>>> dindin.granaPorExtenso('R$897123')
>>> 'oitocentos e noventa e sete mil, cento e vinte e três reais'
```

Also with cents:

```
>>> import dindin
>>> dindin.granaPorExtenso('R$23,27')
>>> 'vinte e três reais e vinte e sete centavos'
```

[Repository of the project.](https://codeberg.org/Buey/Numex/ "Numex number converter.")

