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

When you are ready to submit your changes to us, first make sure you have committed them to your fork of the repo. Then submit a pull request to the `dev` branch of the main `tech.soa.cmu.edu` repo. Here are further details on how to create a [pull request.](https://help.github.com/articles/creating-a-pull-request/)

#### Tag Master List

* cnc
* lasercutting
* grasshopper
* rhino
* rendering
* webdev
* ui-ux
* printing

#### Reference

Create a `.markdown` file in the `_references` folder, where the file name should be unique, following a convention of `organization-product.markdown` ie. `google-fonts.markdown` where a `-` is placed between each word. Below is a sample file for a reference. `title` should be a product name. `link` is the web url for the reference, make sure to include the full url with `http://`. `date` is the date you are publishing this page. `tags` is a list of space seperated tags pull from the tag master list above.
Finally the main section should be a description of the reference.

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

Again create a `.markdown` file, but this time in the `_tutorials` folder. The file name should be unique and be the tutorial name, words seperated by a `-` ie. `cnc-setup.markdown`. If any media files such as images need to accompany this tutorial, they should be held in a folder, with the same name as the tutorial located in the img folder. ie. `img/cnc-setup/`. All tutorials require a thumbnail of size `500px` by `375px`, which should be placed in `img/thumbnails/` folder. Again the file name for the thumbnail should be the same as the tutorial ie. `cnc-setup.png`.

All file names need be lowercase and all files should be `1MB` or smaller where the image length should be no longer then `1400px` on the longer side. `png` files are recommended over `jpg`. You can optimize the images using [imageOptim](https://imageoptim.com/mac) for Mac and [XnView](http://www.xnview.com/en/xnview/) for Windows.


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

{% highlight markdown linenos %}

---
layout: workshop
title: Intro to Design Thinking
details: Prerequisite for UX Series
start-date: 2017-10-05 10:00:00 -0500
end-date: 2017-10-05 10:10:00 -0500
registration: http://registrationlink.com
location: CFA Mac Cluster
instructor: Jony Ive
tags: ui-ux webdev
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean commodo mi dolor, sed lacinia urna lobortis lobortis. Praesent odio dolor, laoreet sed ultricies sed, rutrum eget dolor. Integer congue nisl nec odio accumsan, non interdum justo eleifend. Ut tincidunt lectus ut leo cursus euismod. Nam eu enim et felis ornare suscipit. Nulla at elit ut ipsum porttitor faucibus. Nam non pellentesque quam, quis tempus sem. Nam rutrum vehicula mi. Aliquam odio nunc, facilisis vel lectus bibendum, feugiat pellentesque metus. Etiam sit amet libero et nisi luctus molestie eget sit amet metus. Interdum et malesuada fames ac ante ipsum primis in faucibus. Nulla sed massa et leo accumsan tincidunt. Nam suscipit nisl quam, sed tempus nulla rutrum sit amet. In nec lobortis purus. Duis placerat dignissim lectus. Fusce tristique, leo in hendrerit pellentesque, nisi ante pulvinar nisl, at rutrum libero magna a velit.

{% endhighlight %}