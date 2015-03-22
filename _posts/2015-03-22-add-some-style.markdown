---
layout: post
title:  "Add some style"
date:   2015-03-22 21:28:49
categories: my-first-website
step: 5
---

Our index.html homepage is looking a bit boring. Oh dear. 

You can change its appearance using a CSS file.

<img src="{{site.baseurl}}/assets/add-style.png" />

A CSS file contains the recipe for how the web page should appear.
It's a separate file from the HTML file and it's linked to the HTML file like this:

{% highlight html %}
<link type="text/css" rel="stylesheet" href="css/simple.css">
{% endhighlight %}

1. Open the 'index.html' file in Sublime and locate the link.
Hint: It's the fifth line down!

What this link is telling you is that the appearance of the page is controlled by a stylesheet named 'simple.css', which is located in the 'css' folder.

2. Go into the 'css' folder and locate the file:

3. Make a copy of 'simple.css' and rename it 'home.css'

4. Now change the link in the 'index.html' file so that it points to 'home.css' instead:

{% highlight html %}
<link type="text/css" rel="stylesheet" href="css/home.css">
{% endhighlight %}

5. Save the modified 'index.html' file.

Now open 'index.html' in your browser and 'home.css' in your text editor so that you can see them side-by-side.

The 'home.css' file contains just one statement:

{% highlight css %}
body {
	font-family: sans-serif;
}
{% endhighlight %}

This statement is called a selector and it tells the browser how to format everything inside the body element of the HTML file. What this particular selector is saying is 'set everything inside the body element to a sans-serif font'.

6. 
a. Modify the 'body' selector by adding a rule to include a background image. 

> Can you guess what the selectors will be?

<br />
<br />

{% highlight css %}
body {
font-family: sans-serif;
background-image: 

}
{% endhighlight %}

b. Now let's add a background image!
Remember to save the file and refresh the page when you're done.

{% highlight css %}
body {
font-family: sans-serif;
background-image: url('../images/cool-lee.png');
}
{% endhighlight %}

7
a. Add a selector that says how to format the 'h1' element.

> Can you guess what this selector will be?

<br />
<br />


{% highlight css %}
body {
font-family: sans-serif;
background-image: url('../images/cool-lee.png');
}
{% endhighlight %}

b. Now let's tell the h1 what colour and size to be:

{% highlight css %}
body {
font-family: sans-serif;
background-image: url('../images/cool-lee.png');
}
h1 {
padding: 0.5em;
background-color: black;
color: white;
border-radius: 0.5em;
}
{% endhighlight %}

We've also told it how much space to have around the header (padding) and the border size it should have (border-radius).

Try changing up the style colours and sizes and see what happens!

Remember to save the file and refresh the page with each change.

> Did you notice how the selectors contain a number of individual formatting rules. Each rule is ended by a semi-colon (;) and consists of a property (such as color) followed by a colon (:) and then a value (such as white). Notice, also, that rules are enclosed in curly braces
{ }.