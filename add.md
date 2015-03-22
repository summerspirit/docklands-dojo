# Welcome to the Docklands Dojo website project!

## How-To: Add a Page

Pages are located inside the 

```
_posts
```

directory.

Click

```
_posts
```

and  you will see a list of current pages.

To create a new file, go to 
File
|_
  New File

and a 'Save As' box will appear.

Jekyll organizes posts by chronological order, so your file name should begin with a date later than the dates of the current posts if it is meant to be a later stage in building the project.

The file name should beging with a date in this format:

2015-03-14

then add another dash at the end of that

2015-03-14-

and then add the name of the post title, with dashes instead of spaces between

2015-03-14-add-some-style

Then be sure to add the file extension at the end! This is .markdown.

2015-03-14-add-some-style.markdown

Then click save! 

====
Now that you have an empty page, we have to add a couple more things.

Open any of the other posts that have already been created and copy everything between

---
and
---

including those dashes.

Paste this at the top of your post, like so:

---
layout: post
title:  "Make a home page"
date:   2015-03-12 21:28:49
categories: my-first-website
step: 5
---

This is called front-matter in Jekyll and points to some style and structure cues in the site.

Be sure to change
title
date
step

Step refers to the step number in the project :)
The date should match the date in your Save file name.
The Title will be the Title of the sushi card.


---
layout: post
title:  "The next shiny page"
date:   2015-03-14 21:28:49
categories: my-first-website
step: 6
---
Then you can start typing!

========
## How-To: Add an Image

To add an image, save your desired image in

docklands-dojo/assets

Alternatively, you can open your Finder window to 

docklands-dojo
|_
  assets

and drag and drop your file in there.

! Be sure to name the image something descriptive when you save it, or renae it once you drag and drop it in.

TIP: It's best if files are in .png format.

Now that your image is in the website project folder in the correct place, you can link to it from your post, like this:

```
<img src="{{site.baseurl}}/assets/my-cool-image.png" />
```

Image links will always begin 

    <img src="{{site.baseurl}}/assets/      

and end

    />

You just have to change the filename in the middle:

```
my-cool-image.png
```


