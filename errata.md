# Errata
LinkedIn Learning course - [SEO Foundations](https://www.linkedin.com/learning/seo-foundations-14828080) - by [David Booth](https://www.linkedin.com/learning/instructors/david-booth)


## Chapter 4 
### lesson 3 - Working with canonical URLs and redirects: Technical SEO<br>
   
1. Sadly the instructor skips over explaining the term and use of the "rel canonical meta tag". This missing information makes it near impossible to know what this is without your own research or previous experience.<br>
    NOT PART OF COURSE: 
    <blockquote cite="https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls">
    A rel="canonical" link element (also known as a canonical element) is an element used in the head section of HTML to indicate that another page is representative of the content on the page.
    
    Suppose you want https://example.com/dresses/green-dresses to be the canonical URL, even though a variety of URLs can access this content. Indicate this URL as canonical with these steps:
    
    Add a `<link>` element with the attribute rel="canonical" to the `<head>` section of duplicate pages, pointing to the canonical page. 

    <pre><code>&lt;head>
      &lt;title>Explore the world of dresses&lt;/title>
      &lt;link rel="canonical" href="https://example.com/dresses/green-dresses" />
    &lt;/head></code></pre>
    </blockquote>
    
    Google Documentation on URL canonicalization<br> 
    [What is URL canonicalization](https://developers.google.com/search/docs/crawling-indexing/canonicalization)<br>
    [canonical URL how to](https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls)

2. The instructor fails to explain a Meta Redirect tag<br>
    NOT PART OF THE COURSE: [Meta Redirect definition by ahrefs.com](https://ahrefs.com/seo/glossary/meta-redirect)
    
      <blockquote cite="https://ahrefs.com/seo/glossary/meta-redirect">
      A meta redirect, also known as a meta refresh redirect, instructs a web browser to navigate automatically to a different webpage after a certain amount of time. Unlike typical 301 or 302 redirects, which happen on the server, a meta redirect is a client-side redirect.<br>
      Meta redirects are created by incorporating a specific meta element in the HTML of a web page, usually within the &lt;head> section. For instance:
      <pre><code>&lt;meta http-equiv="refresh" content="7; url=https://ahrefs.com/"></code></pre>
      Meta refresh redirects can be both instant and delayed.
      content="7... in the given example signifies a redirection delay of 7 seconds.
      </blockquote>


3. Chapter 4 quiz
   - question 2 says a color is an on page element that can be optimized. This wording is odd and laughable at best because one color is not "optimized" over another color. The CSS styles can be minimized and optimized. The UI design can be improved for stronger contrast and readability. But you cannot optimize a color.
   
   - question 4 forgets to mention Google Search Console




