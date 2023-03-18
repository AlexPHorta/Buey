
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

[Live preview.](https://www.buey.net.br/nsew/ "NSEW Virtual Keyboard live preview")

[Repository of the project.](https://codeberg.org/Buey/NSEW-Keyboard/ "NSEW Virtual Keyboard on Codeberg")

Numex
======

Get written numbers (and money quantities) from numbers.  In Brazilian Portuguese.  This one I would really love to have enabled in my work (I have to write large money quantities from time to time).

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

