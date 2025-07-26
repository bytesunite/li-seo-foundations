# Chapter 4 - Content Optimization: Technical SEO
## Lesson 3 - Working with Canonical URLs and Redirects: Technical SEO

Search Engines rely on unique URLs as pointers to each piece of content on the web. But often our pages introduce slightly varied URLs for the same piece of content, which can be a problem.<br>
When talking about SEO, the term "duplicate content" is used to describe URL's that are slightly different that point to the same content. Examples of this are URLs that use *url parameters*, which extra data is added to the end of a URL.

<pre>
Example URL Parameter

https://example.com/index.php?id=342
https://example.com/index.php?lang=en
</pre>

In some cases the URL returns unique content from a database using a unique id, identifying the product, article, etc. This is demonstrated above using "?=342". Other times these URL parameters store session data and other pieces of information that does not change the content being displayed. 

There are a couple ways to deal with duplicate URLS
- The "rel" canonical meta tag
- Tools like Google Search Console & Bing Webmaster Tools 
- Redirect rules

Using these allows you to specify URL parameters that should be ignored, helping the Search Engine to ignore duplicate pages.

### The "rel" canonical meta tag
Sadly the instructor quickly skips over what "canonical" means or what a "rel canonical meta tag" is or how it works.<br>

NOT PART OF COURSE:<br>
Google has more details in the links below but lets look at a quick example. If duplicate pages exist, you can specify a specific page is a representation of the duplicate page.
<blockquote cite="https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls">
A rel="canonical" link element (also known as a canonical element) is an element used in the head section of HTML to indicate that another page is representative of the content on the page.

Suppose you want https://example.com/dresses/green-dresses to be the canonical URL, even though a variety of URLs can access this content. Indicate this URL as canonical with these steps:

Add a `<link>` element with the attribute rel="canonical" to the `<head>` section of duplicate pages, pointing to the canonical page. 

<pre><code>&lt;head>
  &lt;title>Explore the world of dresses&lt;/title>
  &lt;link rel="canonical" href="https://example.com/dresses/green-dresses" />
&lt;/head></code></pre>

</blockquote>
EXTERNAL RESOURCES:<br>
[What is URL canonicalization](https://developers.google.com/search/docs/crawling-indexing/canonicalization)<br>
[canonical URL how to](https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls)


### Tools like Google Search Console & Bing Webmaster Tools
The instructor shows how Google Search Console provides a "URL parameters" section, where you can specify which URL parameters should be ignored, such as "sessionId, tracking, _preview, csspath, versionID".

### Redirects
Another reason for duplicate content is when it has been moved from one location to another. The old and new content could potentially be in the search index at the same time. When moving content it is important to implement "redirect rules". These redirect rules are setup by your webmaster on the backend.
- 302 redirect: short-term, temporary content moves
- 301 redirect: long-term, permanent content moves

It is important to know that redirecting pages with JavaScript or Meta Refresh redirects are not always picked up by Search Engines. This instructor says you will generally want to avoid them.<br>

Again, the instructor fails to show an example or go into details.

NOT PART OF THE COURSE: [Meta Redirect definition by ahrefs.com](https://ahrefs.com/seo/glossary/meta-redirect)
<blockquote cite="https://ahrefs.com/seo/glossary/meta-redirect">
A meta redirect, also known as a meta refresh redirect, instructs a web browser to navigate automatically to a different webpage after a certain amount of time. Unlike typical 301 or 302 redirects, which happen on the server, a meta redirect is a client-side redirect.<br>
Meta redirects are created by incorporating a specific meta element in the HTML of a web page, usually within the &lt;head> section. For instance:
<pre><code>&lt;meta http-equiv="refresh" content="7; url=https://ahrefs.com/">
</code></pre>
Meta refresh redirects can be both instant and delayed.

content="7... in the given example signifies a redirection delay of 7 seconds.
</blockquote>