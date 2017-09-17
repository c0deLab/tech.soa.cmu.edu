---
layout: post
title: "HTML & CSS: A Little Deeper"
thumbnail: html-css-little-deeper.png
tile-name: "HTML & CSS: A Little Deeper"
date: 2017-09-16

author: Rehan Butt
tags: [html, css, webdev]
---

## HTML

{% highlight html linenos %}
  <tagname attribute="value">
    content
  </tagname>
{% endhighlight %}

{% highlight html linenos %}
  <a href="http://tech.soa.cmu.edu">
    Here be a link
  </a>
{% endhighlight %}


A good starting place for your `html` files.

{% highlight html linenos %}
  <!doctype html> <!-- instruction to the browser about what version of HTML the page is written in.-->
  <html>
    <head> <!-- title,scripts, styles, meta information, and more. -->
      <meta charset="UTF-8">
      <title>Sample</title>
    </head>

    <body>
    <!-- Content of the Body -->
    </body>
  </html>
{% endhighlight %}

The `<head>` contains `meta` information about the page, information the browser needs before rendering it. While the `<body>` contains the actual viewable contents of the page.

Here are some common html tags:

{% highlight html linenos %}
  <!-- Headlines -->
  <h1>Header 1</h1>
  <h2>Header 2</h2>
  
  <!-- Paragraph -->
  <p>paragraph</p>
  
  <!-- Lists -->
  <ul> <!-- Unordered Lists -->
    <li>List Item 1</li>
    <li>List Item 2</li>
  </ul>
  
  <ol> <!-- Ordered Lists -->
    <li>List Item 1</li>
    <li>List Item 2</li>
  </ol>
  
  <!-- Images -->
  <img alt="Tech SoA Logo" src="http://tech.soa.cmu.edu/img/favicon.png">
  
  <!-- Links -->
  <a href="http://tech.soa.cmu.edu"> Here be a link </a>
  
{% endhighlight %}

Mozilla has great [documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) that outlines many of the HTML elements, play and browse!

Now that we know some of the basics lets create a simple page. Create a page with `meta` description, nav bar, some body content with a couple elements from above or from the Mozilla docs and a footer. Rock and roll!

## CSS

{% highlight css linenos %}
  selector{
    property: value;
  }

  .class{
    property: value;
    property: value;
  }
  
  .class:sudoclass{
    property: value;
  }
  
  #id{
    property: value;
  }
{% endhighlight %}

{% highlight css linenos %}
  .nav{
    padding: 10px;
    margin: 10px;
    background-color: green;
  }
  
  .nav:hover{
    background-color: blue;
  }
  
  #logo{
    width: 200px;
  }
{% endhighlight %}

You are probably thinking there are real color names in css? How is that possible? Well many have been included with the language, that being said you can also use `hex` and `rgba` values. For a full list of supported colors check this [out](https://www.w3schools.com/colors/colors_names.asp). And if you are looking for some other awesome colors check out [Qulr.life](http://qulr.life).


![Padding or Margin?](/img/html-css-little-deeper/padding-margin.png)