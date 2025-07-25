# Chapter 4 - Content Optimization: Technical SEO
## Lesson 2 - Outlining how Search Engines Index Content

Search Engines discover new content on the web by following links with a little help from us, sitemaps & ping services, and some rules we can set for them.

If you want to make sure that Search Engines can find you there are a few steps you can take. Search Engines are busy following every link they can find.

### Make Your New Content Discoverable
1. Make sure your site has links pointing to your content.<br>
   Links from within your sites menu(s), site directory, promotional content, etc. should point to your new content.
2. Leverage XML Sitemaps<br>
   A sitemap is basically an organized list of pages within your site that mirrors you site structure. Most sites have an HTML footer with this information. However, the "Extensible Markup Language" or "XML" is one format you can feed directly to Search Engines. Once you create your XML sitemap you can send them directly to the Search Engines.<br>
   Learn more about building and submitting sitemaps to google:<br>
   - [sitemaps.org/](https://www.sitemaps.org/protocol.html)
   - [Google Search Console](https://search.google.com/search-console/about)
   - [Google Developers Documentation : Build and Submit a Sitemap] https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap
3. Set rules for the search engine<br>
   Think of areas you may NOT want search engines to know about or follow such as members only areas of your website. A "robots.txt" file is used to set these rules. This can help illustrate important pages, it is **important to understand** it will **NOT** prevent Search Engines from indexing or ranking a page.<br>
   To prevent a page from NOT showing up at all, a `<meta name="robots" content="nodindex,nofollow">` tag is used. Google uses a specific meta tag of `<meta name="googlebot" content="noindex,nofollow">`.<br>
   To control how a site is crawled, use "robots.txt"<br>
   To make sure pages do NOT show up in search results use a meta noindex tag.<br>
   Resources:
   - [robotstxt.org](http://www.robotstxt.org/)
   - [Google Developer : Meta tags](https://developers.google.com/search/docs/crawling-indexing/special-tags)


A Search Engine also takes other things into consideration about your website in determining the quality of your website. It is important & best practice to address the following to make sure your website provides quality and trusted content.
- Server uptime
- Page load speed
- Secure you page with HTTPS

To make sure you website gets indexed properly and as fast as possible, remember to:
- use internal linking for Search Engines to follow
- submit a sitemap so Search Engines to quickly understand you site structure
- use a "robots.txt" file to help surface important pages
- use Meta nofollow tags to stop specific pages from displaying in searches
