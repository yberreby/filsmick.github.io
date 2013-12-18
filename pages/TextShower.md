---
layout: page
title: TextShower
excerpt: Super simple, lightweight, Pure JS and CSS text slider.
permalink: /TextShower/
---

### TextShower live example

Here's an example of what TextShower can do. Check the source of this page if you want!

<div class="TextShower-box"> 
<strong class="TextShower-title">Hey, I'm a title! Click me!</strong> 
<p class="TextShower-text">I'm the content of this box. But what if the user has no JavaScript? Well, by default I'm unfolded, so he can still see me.</p>
</div>

<p>I'm a simple paragraph. I'm dynamically moved as the textbox above me unfolds.</p>

<div class="TextShower-box"> 
<strong class="TextShower-title">I'm another title !</strong> 
<p class="TextShower-text">My title doesn't have a '+' in it if there is no Javascript. But if there is and you click it, it will become a '-'! You can customize that in the arguments.</p>
</div>

The margin, the padding and the height of the boxes are animated.

TextShower also handle **anchors**. [Click here](#anchor-box).

<div class="TextShower-box"> 
<strong class="TextShower-title" id="anchor-box">I'm an anchor-triggered box.</strong> 
<p class="TextShower-text">As you can see, when you click me, your browser scrolls to my position and I unfold smoothly. Perfect for very long files! Just give an id to the title of your box and create a link to it to use this feature.</p>
</div>


### Download and instructions
Downloads are on the [releases page](https://github.com/filsmick/TextShower/releases/latest/) and instructions are in the [README](https://github.com/filsmick/TextShower#readme).

<script src="/javascripts/TextShower.min.js"></script>