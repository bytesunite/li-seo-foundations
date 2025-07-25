# Chapter 4 - Content Optimization: Technical SEO
## Lesson 1 - Interpreting the Code Behind Webpages for SEO

A Search Engine is a machine so it can't interpret visuals and text associations as well as people can when it crawls a website. People see rich colors and graphics that aid in separating content, directing the vistors to areas of a page, showing menus, and more. But Search Engines simply can't pick up on these UI features, instead it sees code. A Search Engine focuses on files it needs to display the page like fonts, links, what happens when hovering over elements. It even focuses on things humans don't see such as meta data such as &lt;meta> tags, Schema.org's ld+json data, img alt attributes, etc.

If we look at an example of a view, people can watch the video and understand what it is about. But a Search Engine only sees a block of code, an HTML `<video>` tag. 

In this case a Search Engine can be left in the dark compared to what a person can see. This code is not very descriptive of what the video is about. Even a person can look at this code and wonder what "podcast_teaser" might mean. A tease about what? Who's podcast? etc. 

<pre>
<code>&lt;video controls poster="_video/podcast_poster.jpg" width="512" height="288" preload="none">
  &lt;source src="_video/podcast_teaser.mp4" type="video/mp4" />
  &lt;source src="_video/podcast_teaser.webm" type="video/webm" />
  &lt;source src="_video/podcast_teaser.theora.ogv" type="video/ogg" />
&lt;/video></code>
<pre>

It helps to make sure your code is clean, efficient, and free of errors. This helps both your visitors and Search Engines.

In lesson 3-3 the instructor hints at using "structured data" to help describe elements like the video tag above, but has yet to fully explore this topic. Structured Data is not introduced until lesson 4-4.
