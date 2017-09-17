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

.class:pseudo-class{
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

Here are some common css property value pairs:

{% highlight css linenos %}
.class{
  background-color: #1d5f77;

  /* Text color */
  color: white;

  /* A font family name and a generic family name */
  font-family: Gill Sans Extrabold, sans-serif;

  text-align:center;

  width: 200px;
  width: 30%;

  /* Apply to all four sides */
  margin: 1em;
  /* top | right | bottom | left */
  margin: 5px 10px 5px 10px;
}

/* Selects every other div inside a parent element */
/* even can be replaced with 2n */
div:nth-of-type(even){
  background-color: lime;
} 

a:hover{
  color: orange;
}
{% endhighlight %}

`classes` and `ids` can be called whatever you would like, as long as the first character is not a number. That being said it is good practice to use letters only and use dashes between words for example `nav-item`. Many properties allow for multiple values, some being optional. Mozilla also has great [documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) on css. Check it out!

What if you want to style a list item, `li`, but not all of them, just ones in the `div` with a class of special? Well you can! All you have to do is add a space. Adding a space between selectors gives more specificity when styling. Remember to keep good code style 👍 !

{% highlight html linenos %}
<div class="special">
  <ul>
    <li>Special List Item</li>
  </ul>
</div>

<ul>
  <li>List Item</li>
</ul>
{% endhighlight %}

{% highlight css linenos %}
.special ul li{
  background-color: aqua;
}
{% endhighlight %}

### Colors

You are probably thinking there are real color names in css? How is that possible? Well many have been included with the language, that being said you can also use `hex`, `rgba` and a couple other formats. For a full list of supported colors check this [out](https://www.w3schools.com/colors/colors_names.asp). And if you are looking for some other awesome colors check out [Qulr.life](http://qulr.life).

{% highlight css linenos %}
.class{
  /* Keyword values */
  background-color: aqua;
  background-color: red;

  /* Hexadecimal value */
  background-color: #f3c311;

  /* Hexadecimal value with alpha channel */
  background-color: #11ffee00; /* 00 - fully transparent */
  background-color: #11ffeeff; /* ff - fully opaque */

  /* RGBA value or RGB with alpha channel */
  background-color: rgba(117, 190, 218, 0.0); /* 0.0 - fully transparent */
  background-color: rgba(117, 190, 218, 0.5); /* 0.5 - semi-transparent */
  background-color: rgba(117, 190, 218, 1.0); /* 1.0 - fully opaque */

  /* HSLA value */
  background-color: hsla(50, 33%, 25%, 0.75);
}
{% endhighlight %}

### Fonts

Fonts can be a lot of fun and there are many properties for them. Find some nice web fonts at [Google Fonts](https://fonts.google.com). When using the `font-family` property you can specify a specific font name or a generic family name such as serif, sans-serif, monospace or cursive. When using a generic family name it will use the browser defaults for each.

`font-weight` is another popular font property. There are several build in weights such as `bold` but it is best to use the ones included with the font like `400` & `700` as seen on line 1 below.

When talking about `font-size` there are several differant units to consider `em`, `px`, `pt` & `%` 

* "Ems" `em` are scalable units. An `em` is equal to the current `font-size`, for instance, if the `font-size` of the document is `12px` then `1em` is `12px`, so `2em` is `24px`.

* Pixels `px` are fixed-size units. One problem with pixels are that they do not scale when users override browser font size setting for accessibility.

* Points `pt` are traditionally used in print media. Points are also fixed-size unit. And are not recommended for the web.

* Percentages `%` are scalar or relative by nature. First and foremost, the current font-size is equal to 100% (i.e. 12pt = 100%).

{% highlight css linenos %}
@import url('https://fonts.googleapis.com/css?family=Roboto+Slab:400,700');

font-family: 'Roboto Slab', serif;
font-family: sans-serif; /* Generic family name */

font-weight: 700;

text-align: left;
text-align: center;
text-align: right;
text-align: justify;

text-decoration: underline;
text-decoration: line-through;

{% endhighlight %}

### Padding & Margin

The short answer is margin is on the exterior of a container and padding on the interior. Creating a exterior buffer and interior duffer respectively. Hoepfully the image of Paddington Bear helps, get it get it 😜 ? Padding-ton

![Padding or Margin?](/img/html-css-little-deeper/padding-margin.png)


Now lets style some pages! Play with nesting of elements, importing a font or 2, adjust colors and add a hover effect or 2. And if you are feeling adventurous check out what a `@media` query does, this [link](https://www.w3schools.com/css/css_rwd_mediaqueries.asp) might help. Use it to create a breakpoint and start thinking responsively. Happy deving! 
## Bonus (Part 1): Puns

![titanic css pun](/img/html-css-little-deeper/titanic-css-pun.png)
![ninja css pun](/img/html-css-little-deeper/ninja-css-pun.png)
![harry potter css pun](/img/html-css-little-deeper/harry-potter-css-pun.png)
![hulk css pun](/img/html-css-little-deeper/hulk-css-pun.png)

Source: [saijogeorge.com](https://saijogeorge.com/css-puns/)

## Bonus (Part 2): Markdown

{% highlight markdown linenos %}
# H1
## H2
### H3
#### H4
##### H5
###### H6

Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~


[I'm an inline-style link](https://www.google.com)
![alt text](http://tech.soa.cmu.edu/img/favicon.png)


Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
{% endhighlight %}

Here are some of the highlights of markdown syntax for more view [this](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) resource.