---
title: Minium learns to play with 'Quick, Draw!'
header:
#  image: /assets/images/code.jpg
  teaser: /assets/images/code.jpg
categories:
  - Minium
  - demo
author: rui.figueira
---

This little video shows Minium drawing a penguin in Google AI experiment 'Quick, Draw!':

<iframe src="https://player.vimeo.com/video/194549806" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

Minium will use some auxiliary sites to "learn" how to draw a penguin:

* First, it searches for line drawing images in [Google images](https://images.google.com) and picks the first one
* It uses that image to get its contours using [Contour by José Manuel Pérez](https://jmperezperez.com/contour/)
* That service converts an image into SVG with `polyline` elements, from which Minium can easily extract all lines and corresponding points
* Minium then simplifies lines so that they have less points and therefore are quickier to draw. For that, it uses the javascript library [Simplify.js by Vladimir Agafonkin](http://mourner.github.io/simplify-js)
* Minium can now go back into 'Quick, Draw' and draw points using mouse interactions with offsets based on line points

You can check the code at https://github.com/viltgroup/minium-quickdraw-demo.
