# Chapter 4 - Content Optimization: Technical SEO
## Lesson 4 - Leveraging Structured Data: Technical SEO

Search Engines do a pretty good job at finding and understanding content. However there are some content it struggles with that we can help it with.

Think of the following examples. Typically these have a title, description, the name of the person, date, rating, 
- product reviews
- embedded videos
- recipe

Using "Structured Data" we can help provide the Search Engine some details to help it index the content correctly.

The instructor take you to [Schema.org](https://schema.org) and explains Schema defines the "structure" and "attributes" of all kinds of elements. The Schema.org website is a collection of universal shared vocabulary that was founded by major Search Engine Providers (Google, Microsoft, Yahoo, & Yandex).

Schema provides a special syntax that can be used to help search engines identify specific types of content on your pages (providing more data than it would gather from the code). Schema provides examples such as a recipe [Schema example recipe](https://schema.org/Recipe). If you scroll down the page you wiil see an example without any markup.
<pre><code>
Mom's World Famous Banana Bread
By John Smith, May 8, 2009
&lt;img src="bananabread.jpg" alt="Banana bread on a plate" />

This classic banana bread recipe comes from my mom -- the walnuts add a nice
 texture and flavor to the banana bread.

Prep Time: 15 minutes
Cook time: 1 hour
Yield: 1 loaf
Tags: Low fat

Nutrition facts:
240 calories, 9 grams fat

Ingredients:
- 3 or 4 ripe bananas, smashed
- 1 egg
- 3/4 cup of sugar
...

Instructions:
 Preheat the oven to 350 degrees. Mix in the ingredients in a bowl. Add the
 flour last. Pour the mixture into a loaf pan and bake for one hour.

140 comments:
From Janel, May 5 -- thank you, great recipe!
</code></pre>

Without help, a Search Engine sees this as a bunch of short fragments of text without a clear way to understand its purpose. People can easily identify this as ingredients in a recipe but a Search Engine can not.

Using *JSON-LD* syntax you can explicitly tell a Search Engine this is a "recipe", by providing markup that a Search Engine can use to understand the content.
<pre><code>
&lt;script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Recipe",
  "author": "John Smith",
  "cookTime": "PT1H",
  "datePublished": "2009-05-08",
  "description": "This classic banana bread recipe comes from my mom -- the walnuts add a nice texture and flavor to the banana bread.",
  "image": "bananabread.jpg",
  "recipeIngredient": [
    "3 or 4 ripe bananas, smashed",
    "1 egg",
    "3/4 cup of sugar"
  ],
  "interactionStatistic": {
    "@type": "InteractionCounter",
    "interactionType": "https://schema.org/Comment",
    "userInteractionCount": "140"
  },
  "name": "Mom's World Famous Banana Bread",
  "nutrition": {
    "@type": "NutritionInformation",
    "calories": "240 calories",
    "fatContent": "9 grams fat"
  },
  "prepTime": "PT15M",
  "recipeInstructions": "Preheat the oven to 350 degrees. Mix in the ingredients in a bowl. Add the flour last. Pour the mixture into a loaf pan and bake for one hour.",
  "recipeYield": "1 loaf",
  "suitableForDiet": "https://schema.org/LowFatDiet"
}
&lt;/script>
</code></pre>


This allows Search Engines to identify a large range of topics that is not easily identified by text fragments. This a large list of predefined categories and subcategories. A short list of examples include the following. Browser the [Full Schema Heirarchy](https://schema.org/docs/full.html) or search for a specific term [Organization of Schemas](https://schema.org/docs/schemas.html)
- Event
- Diet
- Book
- Movie
- Guide
- Menu
- HowTo
- Review

Take the example of a "Book" and you will see a Schema with many attributes. Go to the [Organization of Schemas](https://schema.org/docs/schemas.html) and search for "book", and it will take you to the [Book Schema](https://schema.org/Book). You will find a long list of attributes. Below is a quick sample of some Book properties.
- title
- author
- datePublished
- audience
- numberOfPages

Likewise if you searched for "Event" it would take you to the [Event Schema](https://schema.org/Event) with a list of available properties.
- name
- location
- organizer
- startDate
- duration
- audience

So based on what you are targeting, whether that is a local business or a Product, make sure to explore different Schemas to find one that matches your intentions. You may be surprised to learn there are about **800 Schema Types** ready for you to use.

The recommended syntax to use is "JavaScript Object Notation - Linked Data" or "JSON-LD" for short.
