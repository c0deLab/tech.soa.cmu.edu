---
layout: content
title: Contribute
permalink: /contribute/
---

Hello SoA community member. Welcome! This page will give you all you need to know about contributing to this site and letting us know if something is not working right.

### Something Wrong?

If you think you've found a bug open a issue [here.](https://github.com/c0deLab/tech.soa.cmu.edu/issues) You will need a GitHub account to do so. When opening a issue be precise as possible for quickest response. Images / screenshots are great ways to help pass the information along.

### Share Some Awesome Content with the Rest of Us

Add a new reference, tutorial or a workshop. First thing you need to do is create a [GitHub](https://github.com) account if you don't already have one. and fork the `tech.soa.cmu.edu` repository. A fork is a copy of a repository or repo. Forking a repository allows you to freely experiment with changes without affecting the original project.

In the top right corner of the [repository](https://github.com/c0deLab/tech.soa.cmu.edu) page you will see the fork button. From here you can make changes to your copy of the repo. The easiest way to use GitHub on your machine is with the [desktop apps](https://desktop.github.com). The other thing you will need is a text editor, I recommend [Brackets](http://brackets.io) or [Atom](https://atom.io).

Now you want to learn how to write a markdown file. The good think is the syntax is pretty simple. If you want simple text, just write it. Bullets add a `*` to the start of the line. Need to add an image use `![Image Phrase Description](/img/name.png)`. Markdown can also handle many of types of styling. Take a look at [this](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) awesome resource to see how.

When you are ready to submit your changes to us, first make sure you have committed them to your fork of the repo. Then submit a pull request to the `dev` branch of the main `tech.soa.cmu.edu` repo. Here are further details on how to create a [pull request.](https://help.github.com/articles/creating-a-pull-request/)

#### Tag Master List

* cnc
* lasercutting
* grasshopper
* rhino
* rendering
* webdev
* ui ux
* printing
* XX-XXX [Course Number]

#### Reference

Create a `.markdown` file in the `_references` folder, where the file name should be unique, following a convention of `organization-product.markdown` ie. `google-fonts.markdown` where a `-` is placed between each word. Below is a sample file for a reference. `title` should be a product name. `link` is the web url for the reference, make sure to include the full url with `http://`. `date` is the date you are publishing this page. `tags` is a list of comma seperated tags pulled from the tag master list above. Finally the main section should be a description of the reference.

{% highlight markdown linenos %}

---
layout: post
title: "Dzgn.IO Toolkit"
link: "http://toolkit.dzgn.io"
date: 2017-03-05
tags: webdev
---

A open set of web development resources to help you develop better and quicker with simple styling blocks.

{% endhighlight %}

#### Tutorial

Again create a `.markdown` file, but this time in the `_tutorials` folder. The file name should be unique and be the tutorial name, words seperated by a `-` ie. `cnc-setup.markdown`. If any media files such as images need to accompany this tutorial, they should be held in a folder, with the same name as the tutorial located in the tutorial folder in the img folder. ie. `img/tutorials/cnc-setup/`. All tutorials require a thumbnail of size `500px` by `375px`, which should be placed in `img/thumbnails/` folder. Again the file name for the thumbnail should be the same as the tutorial ie. `cnc-setup.png`.

All file names need be lowercase and all files should be `1MB` or smaller where the image length should be no longer then `1400px` on the longer side. `png` files are recommended over `jpg`. You can optimize the images using [imageOptim](https://imageoptim.com/mac) for Mac and [XnView](http://www.xnview.com/en/xnview/) for Windows.

`date` should be the publish date following the `YYYY-MM-DD` convention. `tile-name` is a short version of the tutorial name that appears on hover of the thumbnail tile. `author` being your name.

{% highlight markdown linenos %}

---
layout: post
title: CNC Setup
thumbnail: tid.png
tile-name: CNC Setup
date: 2017-03-05

author: Rehan Butt
tags: cam branding
---

![Hero Image](/img/test/hero.png)

Your short description goes here. 100 word max.

this is what an image looks like
![2 Word Image Description](/img/test/thisImage.png)

this is what a video embed looks. please update width to be `100%` otherwise it will break on mobile devices.

<iframe src="https://www.youtube.com/embed/IdneKLhsWOQ" frameborder="0" allowfullscreen></iframe>

and this is how you include a link into stuff [link](http://cmu.edu). want to see where the link goes?

{% raw %}{% highlight html linenos %}{% endraw %}
<!--This is what a code block looks like.-->
<iframe width="100%" height="600" src="https://www.youtube.com/embed/w0ZcpQ547Gg?rel=0" frameborder="0" allowfullscreen>
</iframe>
{% raw %}{% endhighlight %}{% endraw %}

{% endhighlight %}


#### Workshop

Again create a `.markdown` file, this time in the `_workshops` folder. The file name should be unique and be the name of the workshop, words seperated by a `-` ie. `intro-design-thinking.markdown`. `start-date` is the start date and time of the workshop follwing the convention `YYYY-MM-DD HH:MM:SS TIMEZONE`. The same convention applies for the `end-date`. `location` being the location of the workshop ie. `Hunt Basement Cluster` or `dFab`. And the `instructor` being the instructor or instructors ie. `Jony Ive` or `Jony Ive &  Harry Potter`.

{% highlight markdown linenos %}

---
layout: workshop
title: Rhino Basics
details: Get familiar with the interface; Practice simple modeling tasks.
start-date: 2017-08-14 09:00:00 -0400
end-date: 2017-08-14 13:00:00 -0400
registration: llink
location: CFA 214
instructor: Eddy Man Kim
tags: [Digital Representation, Rhino]
---

More workshop content will be posted here.

{% endhighlight %}