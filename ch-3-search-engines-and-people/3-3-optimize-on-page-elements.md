# Chapter 3 - Content Optimization for SEO: How Search Engines and People View Webpages
## Lesson 3 - Optimizing on-page Elements

**On-page Optimization** is the process of fine tuning the relevance of a page for a certain keyword or search term.

To provide an example of how this works the instructor circles back to a previous lesson using the tour site "explorecalifornia.org/tours/tour_detail_backpack.html".<br>
To optimize this page for the keyword phrase "backpacking tours in california" we could do the following.

### Optimize the page url
First, optimize the url.<br>
It can be tricky to find a good balance of useful keywords and url length.<br>
For example if we want to use the phrase "backpacking tours in california" we could optimize the page as follows.
<pre>
BEFORE: tour_detail_backpack.html

AFTER: backpacking-tours-in-california.html
</pre>

### Optimize the page &lt;title>
Next, make sure the HTML &lt;title> tag for the page describes the content.<br>
Right now the title does not give the Search Engine any information to match it to the keyword phrase of "backpacking tours in california". Notice how we didn't just repeat the same keyword phrase. A good guideline is around 65 characters.
<pre>
BEFORE: &lt;title>A little about us...&lt;/title>

AFTER: &lt;title><span style="color:green">Backpacking tours in California - Explore California</span>&lt;/title>
</pre>

The hyphen at the end "- Explore California" was used because the &lt;title> is commonly used for the page's Search Engine results listing. Not only are we trying to optimize the title so that Search Engines identify the theme of the page, it is also used to entice users to click on it.<br>
Just know that Search Engines, like Google, might rewrite this title if it believes it does not match the search query or content on the page.

### meta description tag
The `<meta name="description" content="Page description. about 156 characters">` HTML tag is used to provide a description to your Search Engine results listing. A good guideline is around 156 characters<br>
This is often ignored by Search Engines and will not improve your rankings. This can however improve the "clickthrough" rate which can positively impact ratings over time. This description is typically what the Search Engine results listing displays after the title.
<pre>
Search Engine Results Listings follow a general pattern

URL
Title
Description
</pre>

### The meta keywords tag
The meta keywords tag is ignored by most Search Engines and is not much help anymore. This is due to a history of <span style="color:red">abuse</span> by web developers using keywords inappropriately to improve Search Engine results rankings regardless of whether the keywords match their content.<br>
<pre><code>&lt;meta name="description" content="An example of HTML5 and CSS3">

&lt;meta name="keywords" content="html5, css3, lynda, local storage, canvas, semantics">
</code></pre>

### h1 header tag
The main header on a page should describe what the content is about. It is important to accurately describe the content and match the keyword phrase, rather than a vague or trendy tagline.
<pre>
BEFORE: <code>&lt;h1>Explore California&lt;/h1></code>

AFTER: <code>&lt;h1><span style="color:green">Backpacking Tours in California provided by Backpack Cali</span>&lt;/h1></code>
</pre>


### page content
The last piece of the puzzle is your page content. It should be written for people first rather than a Search Engine. This makes the content engaging. For a Search Engine it might make sense for it to search for common word associations in the content such a "backpack, trip, map, tent, outdoors, vacation, etc.". Search Engines are getting better at interpreting natural language such as themes & semantics. Don't overthink it and focus on making the content read naturally for your human readers.

### putting it all together
There is no perfect formula for a Search Engine. But, with all these different pieces now aligning with our original keyword phrase of "backpacking tours in california" a Search Engine will see a pattern and gain insights into what your page is all about.

### other ways to improve SEO on pages
Although a.i. and machine learning is improving, humans are still better at interpreting colors and text in images that computers. But there are other elements on a page where you can provide descriptions of visual content.

#### image tag
The HTML `<img>` tag includes a "src" attribute with a path to the file, and an "alt" attribute with a description used by screenreaders and adds accessibility to the page.<br>

First, you can rename the image file to better describe it's content.
<pre>
BEFORE: <code>&lt;img src="../images/backpack_main.jpg" alt="Backpack Cali"></code>

AFTER: <code>&lt;img src="<span style="color:green">../images/backpacking-tours-in-california.jpg</span>" alt="Backpack Cali"></code>
</pre>

Second, you can take advantage of the "alt" attribute description.
<pre>
BEFORE: <code>&lt;img src="../images/backpacking-tours-in-california.jpg" alt="Backpack Cali"></code>

AFTER: <code>&lt;img src="../images/backpacking-tours-in-california.jpg" alt="<span style="color:green">Backpacking Tours in California by Backpack Cali</span>"></code>
</pre>

#### proximity of text to non text elements
When you are using content other than text it helps to have text around it. Examples include text next to videos, paragraphs with embeded images can have text below them, image slide shows or carousels often have text below them, audio typically has a text description around them or a complete transcription of the audio. 

### Structured data
The instructor does not go into details at this time.<br>
**Structured Data** is a way to provide specific meta data to specific kinds of content, such as videos. By adding special markup using guidelines on Schema.org with JSON-LD code, you can add meta data to elements like a video tag. The following **structured data** example will allow a video to show up in search results for a keyword search such as "Explore California Videos".

<pre>
<code>&lt;video controls poster="_video/podcast_poster.jpg" width="512" height="288" preload="none">
  &lt;source src="_video/podcast_teaser.mp4" type="video/mp4" />
  &lt;source src="_video/podcast_teaser.webm" type="video/webm" />
  &lt;source src="_video/podcast_teaser.theora.ogv" type="video/ogg" />
&lt;/video></code>

<code>&lt;script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "VideoObject",
  "name": "Explore California video podcast",
  "description": "A new commercial for the Explore California podcast, highlighting beautiful scenery, plenty of places to ride bikes, beautiful weather and more!",
  "thumbnailUrl": "http://explorecalifornia.org/tour-california-podcast.jpg",
  "uploadDate": "2022-01-01T15:00:00.00Z",
  "duration": "T1M33S",
  "contentUrl": "http://www.explorecalifornia.org/_video/podcast_teaser.mp4"
}
&lt;/script>
</code></pre>

To test this, it is suggested to validate it using **Google Rich Results Test** or **Schema Markup Validator**.
