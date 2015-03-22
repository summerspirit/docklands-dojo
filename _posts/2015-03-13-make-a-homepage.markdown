---
layout: post
title:  "Make the home page"
date:   2015-03-13 20:28:49
categories: my-first-website
step: 4
---


###Step 1
Go into the `my-first-website` folder, copy the `about-me.html` file (again!) and this time rename it `index.html`

`index.html` will be the Home page for your site.

Home pages are often given a file name of `index.html`

> Hint: Go back to [Step Three: Make a New Web Page](http://docklandsdojo.github.io/docklands-dojo/my-first-website/2015/03/12/make-a-new-webpage.html)

###Step 2
Edit `index.html` so that it's like the one in the screenshot below (except that it has your name in it, not Lee’s)

<img src="{{site.baseurl}}/assets/create-homepage.png" />


The `index.html` page has two links on it. If you click one of the links you are taken to one of the pages you made earlier.
A link has two main parts —

<img src="{{site.baseurl}}/assets/create-homepage-links.png" />


Also, be careful when you're typing links. You have to get them exactly right!
They always have the same pattern — start and end a tags —

{% highlight html %}
<a href="filename">Link text</a>
{% endhighlight %}

Notice that the starting a tag is inside the same set of < > as href and the filename, which is different than the ending a tag, which is all by itself.

####For example

{% highlight html %}
<a href="about-me.html">About Me</a>
{% endhighlight %}

Notice how the href attribute puts quote marks `" "` around the filename and how it comes inside the a start tag.

##Your challenge

Make three more pages and add the links from the Home page.



Some suggestions: 
(Your own ideas welcome too!)

| Title  | File Name |
|---|--- |
|  My Family | family.html |
| My Pets  |  pets.html |
|  My Top Songs | songs.html |
|  My Hobbies | hobbies.html |
|  My Heros | heros.html |
