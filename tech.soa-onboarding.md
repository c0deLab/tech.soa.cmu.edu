---
layout: content
permalink: /onboarding/
---

Welcome to the documentation for my work in Spring 2020. For whoever works on the site next, I hope this helps with the tech.soa onboarding. 😇

With Love,
Selena Zhen

---

## **Basics**

tech.soa is built using [Jekyll](https://jekyllrb.com/), and hosted through [GitHub](https://github.com/c0deLab/tech.soa.cmu.edu). If you're working on the site, you'll need to do a few things in order to run the site locally. 

1. Create a GitHub account and clone the [repo](https://github.com/c0deLab/tech.soa.cmu.edu) on your computer
2. Set up a [dev environment](https://jekyllrb.com/docs/installation/#requirements)
4. Run the site using `jekyll s` (in the terminal or on GitHub command line)
3. Edit and have fun. 😎

**The frontend uses the [Foundation](https://get.foundation/sites/docs/) framework.** It's similar to Bootstrap, Semantic UI, or other similar systems. This site really only uses the framework's [Grid](https://get.foundation/sites/docs/grid.html) system, which is a 12-column, nestable Foundation grid.

**Additionally, you may need to learn more about the [Liquid Coding Language](https://shopify.github.io/liquid/)** to work with making/editing how dynamic content works.

---

## **Site Structure**

Jekyll puts the site together with a kit of parts/templates that can be reused over and over again. To edit certain things, see the following locations:

- Home page - `index.html`
- Nav Bar - `_includes/header.html`
- HTML head (metadata and head elements) - `_includes/head.html`
- Footer Banner - `_includes/footer.html`
- Templates for page layouts in `_includes` folder
	- Posts (for individual softwares, posted tips, references, tutorials, etc) `_layouts/post.html`
	- Pages (for pages that compile softwares, posted tips, references, tutorials) `_layouts/page.html`
	- etc!
- CSS: This site uses SASS. `css/tech.scss`
- All main pages, such as `tech.soa.cmu.edu/software`, `tech.soa.cmu.edu/tags`, `tech.soa.cmu.edu/tips`, `tech.soa.cmu.edu/tutorials`, and `tech.soa.cmu.edu/workshops`, are located in the general repo folder, named such as `software.html`. 

![All Files in Repo](../img/onboarding/allfiles.png "All Files in Repo")

---

## **Buckets of Markdown Pages**

All of the dynamic content on the site are placed in 'buckets' that each page calls for (using Liquid). For example, all markdown software pages are placed in the bucket `_software`, which `software.html` calls for. See the following image for an example of how it calls for each item, and for specific meta data within each item.  

![For Loop](../img/onboarding/forloop.png "For Loop")

Within each markdown file in a bucket is a set of metadata that you can call for in the for loops. See the following images as examples of data that can be set for each item. 

![Markdown Metadata Example 1](../img/onboarding/example1.png "Markdown Metadata Example 1")  

![Markdown Metadata Example 2](../img/onboarding/example2.png "Markdown Metadata Example 2")

Following that metadata information is the rest of the page. Fill out this space as you would for any markdown document. The following image is what the site creates based on the markdown file. 

![Complete Markdown Page Example](../img/onboarding/completepage.png "Complete Markdown Page Example")

When creating a new page, be sure to follow the same format as the other pages in the bucket, with the same metadata information and page hierarchy. Name the markdown file similarly, and make sure it is in the correct bucket. This will ensure graphic consistency as well as the site's ability to maintain the right information on the right pages. 

---

## **Tags**

Note the tags in the metadata for each markdown page -- this is used to create a navigational index of the entire website in the [Tags](../tags/) page. This pulls from all buckets to ensure that everything is represented. 

![Tags Page Example](../img/onboarding/tagspage.png "Tags Page Example")

Be sure to add these tags in the metadata in order to ensure the Tag page is automatically and dynamically updated. Be as descriptive as possible, and reference the Tags page if you need inspiration!

---

## **Posted Tips**

The posted tips page was created as a compilation of posts from the VTF members' posts on Slack. The page serves as an index for all posts, which one can navigate via post name. Additionally, the page allows as a continuous feed for all posted tips, for casual browsing. 

![Posted Tips Page Example](../img/onboarding/postedtips.png "Posted Tips Page Example")

In the future, I hope that all of the great gif content created on Slack can be migrated here, in the form of Markdown files. Luckily the buckets and format of the site make that easy. 

---

## **Styles**

Other than working on the site structure, a lot of time was spent on visual elements, such as tidying up the styles, adding more dynamic interactions, and page hierachy. 

One thing to note, is that all basic links (`<a href="...">...</a>` without a class) have been styled with the green tech-accent color, in order to allow the link interactions to appear on the individual markdown post pages. Unfortunately, that just means that if you want a link that looks black, then turns green on hover, use the class `blackLink`. 


> An example of a Basic Link:  
>
> `<a href="..."> ... </a>`
>
> ![Basic Link Example](../img/onboarding/basiclink.gif "Basic Link Example")

<br>

>An example of a link with a `blackLink` class: 
>
>`<a href="..." class="blackLink"> ... </a>`
>
>![Basic Link Example](../img/onboarding/blackLink.gif "Basic Link Example")

---

## **Accessibility**

Lastly, be sure to include information within the pages (both in html and markdown) that help with accessibility! Things like titles and alt text help with images and link accessibility, such as if images don't load, and so descriptions appear on hover. This is a good practice to include in all webites, so don't forget! 


