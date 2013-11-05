---
layout: page
title: TextShower
excerpt: Super simple, lightweight, Pure JS and CSS text slider.
---

``` html
<div class="highlight highlight-html"><pre><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"TextShower-box"</span><span class="nt">&gt;</span> 
<span class="nt">&lt;strong</span> <span class="na">class=</span><span class="s">"TextShower-title"</span><span class="nt">&gt;</span>Title<span class="nt">&lt;/strong&gt;</span> 
<span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"TextShower-text"</span><span class="nt">&gt;</span>Content<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;/div&gt;</span>
</pre></div>
```

###Welcome to TextShower

TextShower is an alternative to all these heavy, hard to use jQuery scripts that slow down the client and the server. TextShower lets you create super simple sliders and customise them in an easy way. Example :

<div class="TextShower-box"> 
<strong class="TextShower-title">Hey, I'm a title! Click me!</strong> 
<p class="TextShower-text">I'm the content of this box. If the user hasn't Javascript enabled, I will be showed. Search Engines can see me. Optimal accessibility!
</div>

I'm a simple paragraph. I'm dynamically moved if the textbox above me unfolds. Yeah, no visual bugs, nothing at all. This is the power of CSS3 transitions! No need of jQuery, uh?

<div class="TextShower-box"> 
<strong class="TextShower-title">I'm another title !</strong> 
<p class="TextShower-text">My title doesn't have a '+' in it if there is no Javascript. But if there is and you click it, it will become a '-'! You can customize that in the arguments.<br>
Div, strong and p are the most suitable HTML tags to use.<br />

</div>

The margin, the padding and the height are animated. 

<div class="TextShower-box">
<h3 class="TextShower-title" id="how-to-use">How to use</h3>

<div class="TextShower-text">
Upload TextShower.js or TextShower.min.js to your FTP server
All you need is this code :

<div class="highlight highlight-html"><pre><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"TextShower-box"</span><span class="nt">&gt;</span> 
<span class="nt">&lt;strong</span> <span class="na">class=</span><span class="s">"TextShower-title"</span><span class="nt">&gt;</span>Title<span class="nt">&lt;/strong&gt;</span> 
<span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"TextShower-text"</span><span class="nt">&gt;</span>Content<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;/div&gt;</span>
</pre></div>

Then embed the script at the end of the code : 

<div class="highlight highlight-html"><pre><span class="nt">&lt;script </span><span class="na">src=</span><span class="s">"path/to/TextShower.js"</span><span class="nt">&gt;&lt;/script&gt;</span>
</pre></div>

<strong>...and you're done!</strong>

If you want to customise the script behavior, go to the <a href="#advanced-usage">Advanced usage</a> section.

</div>
</div>

<div class="TextShower-box">
<h3 class="TextShower-title" id="advanced-usage">Advanced usage</h3>

<div class="TextShower-text" markdown="1">
Settings are set in two steps : in the .js file, and in a custom meta tag. You can specify general settings in the file and page-wide settings in the meta tag, that will overwrite the general ones. 

<strong>General settings</strong>

Edit the <code>TextShower()</code> function at the end of the script file. The first argument is text transition duration, second is margin transition
duration, third is text transition timing function, fourth is margin transition timing function and fifth is a boolean that means "should we add a
dynamic '+' sign to the box title".
Default values are respectively <strong>0.8s</strong>, <strong>0.3s</strong>, <strong>ease</strong>, <strong>linear</strong> and <strong>true</strong>.

Function template:

``` javascript
TextShower('0.8s', '0.3s', 'ease', 'linear', true);
```

<br />
<strong>Local settings</strong>

Custom meta tag template:

```
<meta data-TextShower="0.8s 0.3s ease linear true" />
```h

Just add this tag to your webpage's header and edit it. The arguments are in the same order than for the function. You can change only some settings by writing <strong>none</strong> where you want a default behavior.

TextShower can handle anchors. If the anchor is the title element, its box will unfold at page load.
</div>
</div>

<div class="TextShower-box">
<h3 class="TextShower-title" id="caveat">Caveat</h3>

<p class="TextShower-text">The content of the text boxes may brievely show up during the page load. It's because the Javascript loads after the HTML, so the content gets hided after the loading is completed. You can choose to have a smooth animation at load by customising the function's arguments, but most of the time this problem doesn't occur.
</div>

<h3>
Credits</h3>

Made by <a href="https://github.com/filsmick" class="user-mention">@filsmick</a> with <strong>Sublime Text 2</strong> and GitHub.
If you like TextShower and want it and all my projects to grow, you can flattr me with the button below.
<script id='fbt8xsh'>(function(i){var f,s=document.getElementById(i);f=document.createElement('iframe');f.src='//api.flattr.com/button/view/?uid=filsmick&button=compact&url=http%3A%2F%2Fgithub.com%2Ffilsmick';f.title='Flattr';f.height=20;f.width=110;f.style.borderWidth=0;s.parentNode.insertBefore(f,s);})('fbt8xsh');</script>

<script src="http://filsmick.github.io/TextShower/TextShower.js"></script>