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
<p class="TextShower-text">My title doesn't have a '+' in it if there is no Javascript. But if there is and you click it, it will become a '-'! You can customize that in the arguments.<br>
Div, strong and p are the most suitable HTML tags to use.<br />
</p>
</div>

<p>The margin, the padding and the height are animated. </p>

<div class="TextShower-box">
<h3 class="TextShower-title" id="how-to-use">How to use</h3>

<div class="TextShower-text">
<p>Upload TextShower.js or TextShower.min.js to your FTP server</p>
<p>All you need is this code :</p>

<div class="highlight highlight-html"><pre><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"TextShower-box"</span><span class="nt">&gt;</span> 
<span class="nt">&lt;strong</span> <span class="na">class=</span><span class="s">"TextShower-title"</span><span class="nt">&gt;</span>Title<span class="nt">&lt;/strong&gt;</span> 
<span class="nt">&lt;p</span> <span class="na">class=</span><span class="s">"TextShower-text"</span><span class="nt">&gt;</span>Content<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;/div&gt;</span>
</pre></div>

<p>Then embed the script at the end of the code : </p>

<div class="highlight highlight-html"><pre><span class="nt">&lt;script </span><span class="na">src=</span><span class="s">"path/to/TextShower.js"</span><span class="nt">&gt;&lt;/script&gt;</span>
</pre></div>

<p><strong>...and you're done!</strong></p>

<p>If you want to customise the script behavior, go to the <a href="#advanced-use">Advanced use</a> section.</p>

</div>

<div class="TextShower-box">
<h3 class="TextShower-title" id="advanced-use">Advanced use</h3>

<div class="TextShower-text">
<p>Settings are set in two steps : in the .js file, and in a custom meta tag. You can specify general settings in the file and page-wide settings in the meta tag, that will overwrite the general ones. </p>

<strong>General settings</strong>

<p>Edit the <code>TextShower()</code> function at the end of the script file. The first argument is text transition duration, second is margin transition
duration, third is text transition timing function, fourth is margin transition timing function and fifth is a boolean that means "should we add a
dynamic '+' sign to the box title".
Default values are respectively <strong>0.8s</strong>, <strong>0.3s</strong>, <strong>ease</strong>, <strong>linear</strong> and <strong>true</strong>.</p>

<p>Function template:</p>

<div class="highlight highlight-javascript"><pre><span class="nx">TextShower</span><span class="p">(</span><span class="s1">'0.8s'</span><span class="p">,</span> <span class="s1">'0.3s'</span><span class="p">,</span> <span class="s1">'ease'</span><span class="p">,</span> <span class="s1">'linear'</span><span class="p">,</span> <span class="kc">true</span><span class="p">);</span>
</pre></div>

<br />
<strong>Local settings</strong>

<p>Custom meta tag template:</p>

<div class="highlight highlight-html"><pre><span class="nt">&lt;meta</span> <span class="na">data-TextShower=</span><span class="s">"0.8s 0.3s ease linear true"</span> <span class="nt">/&gt;</span>
</pre></div>

<p>Just add this tag to your webpage's header and edit it. The arguments are in the same order than for the function. You can change only some settings by writing <strong>none</strong> where you want a default behavior.</p>

<p>TextShower can handle anchors. If the anchor is the title element, its box will unfold at page load.</p>
</div>

<div class="TextShower-box">
<h3 class="TextShower-title" id="caveat">Caveat</h3>

<p class="TextShower-text">The content of the text boxes may brievely show up during the page load. It's because the Javascript loads after the HTML, so the content gets hided after the loading is completed. But don't worry, most of the time it don't happens, or only at the first connection.</p>
</div>

### Download
Latest stable version: <a href="/javascripts/TextShower.js" download>Download</a>  
Latest stable minified version: <a href="/javascripts/TextShower.min.js" download>Download</a>  
*Do a right click on the link and select "Save as..." or "Download linked file as..." to download*

If you want to have the very newest builds, simply [download the master branch](https://github.com/filsmick/TextShower/archive/master.zip) of the repository. You will find TextShower.js, TextShower.min.js, an HTML test page, the license and the readme. Be careful! Some things may be broken because these builds are not fully tested.  

Feel free to edit the code to achieve your goals. It's open source, after all!

### Credits

Made by <a href="https://github.com/filsmick" class="user-mention">@filsmick</a> with <strong>Sublime Text 2</strong> and GitHub.  
If you like TextShower and use it regularly, you can flattr me with the button below.  
<script id='fbt8xsh'>(function(i){var f,s=document.getElementById(i);f=document.createElement('iframe');f.src='//api.flattr.com/button/view/?uid=filsmick&button=compact&url=http%3A%2F%2Fgithub.com%2Ffilsmick';f.title='Flattr';f.height=20;f.width=110;f.style.borderWidth=0;s.parentNode.insertBefore(f,s);})('fbt8xsh');</script>

<script src="/javascripts/TextShower.js"></script>
