---
layout: post
title:  "2. Edit a Webpage"
date:   2015-03-15 20:28:49
categories: my-first-website
---


###Step 1
Go into the `my-first-website` folder and open the `about-me.html` file.
<img src="/assets/edit-webpage-open.png" />
_It opens in your web browser._

###Step 2
Now open the same file in a text editor such as Sublime.

###Step 3
Arrange the Browser window and the text editor window so that they are alongside one another on your screen.
<img src="/assets/edit-page-sublime-browser.png" />


###Step 4
Change the text in the page so that it’s about you — not _Lee Go_.

###Step 5
After you have changed some text, save the file in Sublime and then refresh the web page in your browser window. To do this click the Refresh symbol.

<img src="/assets/edit-page-refresh.png" width="60%" />

_What happens?_

###Step 6
Now put in a new paragraph of text. This needs to go between the <p> and </p> tags.
Like this:
{% highlight css %}
<p>I am learning how to make a website at CoderDojo.</p>
<p> is the start tag for a paragraph element, </p>
{% endhighlight %}
is the end tag.


###Step 7
Again, Save and Refresh.
You can see now that a web page is just text typed into a text file. How the text appears on the web page is controlled by the tags.
* What happens if you use h1 or h2 elements instead of p?
* What happens if you put some words inside strong? Like this:

{% highlight css %}
<p>My name is <strong>Lee Go</strong></p>
{% endhighlight %}


<a href="{% post_url 2015-03-15-make-a-new-webpage %}" class="btn next-step pull-right">Next Step: Make a new web page</a>

