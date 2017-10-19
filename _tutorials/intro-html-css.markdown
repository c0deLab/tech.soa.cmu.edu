---
layout: post
title: Intro to HTML & CSS
thumbnail: intro-html-css.png
tile-name: Intro to HTML & CSS
date: 2017-09-12

author: Rehan Butt
tags: [html, css]
---

## Background / Potentially Fun Facts

#### The world is run on the web
#### 2.5 [Exabytes](https://en.wikipedia.org/wiki/Exabyte) of data are created each day, much of it is rich multimedia
* Knowing how to create data is one thing
* Knowing how to effectively share it in a manner that others can understand sets you apart


![ARPANET September 1971](/img/intro-html-css/arpanet.png)
Source: [California State University](http://som.csudh.edu/fac/lpress/history/arpamaps/f8sep1971.jpg)


### Web 1.0

* Focused on efficient delivery of static content (sharing information rather than rich multimedia)
* User experience was not a focus (web use required more technical skills)
* Pages were written in basic HTML with little to no styling
* Companies were the sole content creators

![Apple.com 1996](/img/intro-html-css/apple.jpg){: style="width=100%;" }

Source: [Telegraph](http://www.telegraph.co.uk/technology/6125914/How-20-popular-websites-looked-when-they-launched.html)

### Web 2.0

* **More Interactive**: Highlight, hover, other visual effects
* **Focus on User Experience**: Animations and transitions
* **Multimedia Focus**: Facebook, Twitter YouTube
* **Far greater number of content creators**: anyone with a computer

![Apple.com 2017](/img/intro-html-css/apple-today.png)

### A Couple Other Things
[Brief History of the Web](https://webdesign.tutsplus.com/articles/a-brief-history-of-the-world-wide-web--webdesign-8710)

[Evolution of the Web](http://www.evolutionoftheweb.com)

## Hacking Webpages

Use the web inspector in your browsers (Chrome, Safari) to manipulate the HTML and CSS of current web pages to see live the effect of the changes that you make
(right click → inspect element)

try hacking these sites:
* [Processly](https://processly.io)
* [Penguin.rehanbutt.com](http://penguin.rehanbutt.com)
* [Wayfair](https://www.wayfair.com)

## Page Makeup

<div class="row">
  <div class="small-12 medium-4 column" style="background-color: #9EC6E6; padding: 20px; text-align: center;">
    <strong>HTML</strong> <br>
    HyperText Markup Language
    <br><br>
    <img src="../img/intro-html-css/structure.png">
    <br><br>
    <strong>Structure</strong>
  </div>
  <div class="small-12 medium-4 column" style="background-color: #B5D7AB; padding: 20px; text-align: center;">
    <strong>CSS</strong> <br>
    Cascading Style Sheet
    <br><br>
    <img src="../img/intro-html-css/style.png">
    <br><br>
    <strong>Styling</strong>
  </div>
  <div class="small-12 medium-4 column" style="background-color: #EB969A; padding: 20px; text-align: center;">
    <strong>JS</strong> <br>
    JavaScript
    <br><br>
    <img src="../img/intro-html-css/interaction.gif">
    <br><br>
    <strong>Interaction</strong>
  </div>
</div>

### HTML
HTML (HyperText Markup Language) is the most basic building block of the Web. 
It describes and defines the content of a webpage. HTML elements are represented by tags.

Written using tags enclosed in angle brackets

`<html>` called opening tag

`</html>` called closing tag

`<!-- comment -->`

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


### CSS

Cascading Style Sheets (CSS) are a stylesheet language used to describe the presentation of a document written in HTML or XML (including XML dialects like SVG or XHTML). CSS describes how elements should be rendered on screen, on paper, in speech, or on other media.

Defined using Classes `.name` and IDs `#name`

Classes: more general, used for a group of elements

IDs: more specific, used for single elements 

`/*comment*/`

`//comment`

{% highlight css linenos %}
  html, body, h1, h2, h3, h4, h5, h6{
    font-family: 'Lato', sans-serif;
    color: black;
  }

  .post-content h4{
    font-size: 22px;
  }

  .page-content{
    margin-left: 10px;
    margin-right: 10px;
  }
{% endhighlight %}

### Content v Styling
Content and style can and should be handled seperately.

Content lives in `.html` files and styling in `.css`

If you think about it in relation to a newspaper `html` is the raw article text and the `css` transforms it into what you get at a newsstand

### Server v Client

Servers give out information (.com’s)

Clients read in the information (web browser)

These can be compartmentalized, services can be both servers and clients

* log into facebook, [facebook = server]
* facebook asks spotify for info [facebook = client]


### Debugging

A lot of bugs come from missing notation, HTML is a very relaxed language, it is not great at telling you where errors are or if there are bugs, it just assumes what should have been.

The web inspector can help understand the hierarchy that makes up HTML files helping you debug.



## Structure & Organization

### Version Control

![git structure diagram](/img/intro-html-css/git.svg)

Basically version control is the bomb! Check this out for a bit more: [Using git #versionControl](git)


### File Structure

![File Structure](/img/intro-html-css/file-structure.svg)

The critical thing with file structure is to stay organzied and be consistent


### Optimize your Code

* Clean and clarify code
* Delete unwanted resources and code
* Have as few files as possible
* Comment to clarify your code
* Browsers load files linearly
* Be consistent

### Image Preparation

* 150 dpi is plenty for the web
* Make images the size you want to display them
* PNGs are good for images
* SVGs for things like logos
* GIFs for animations
* All of the file types above supports transparency!
* Optimize your images: [imageoptim (mac)](https://imageoptim.com/mac) [xnview (win)](http://www.xnview.com/en/)
* Recommend using `word-space.png` for file names


Also check out [HTTParty](https://dzgn.io/works/httparty.html) for a little extra, much of this content was pulled from there.