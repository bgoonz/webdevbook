---
description: Structuring the web with HTML
---

# Html

To build websites, you should know about [HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML) — the fundamental technology used to define the structure of a webpage. HTML is used to specify whether your web content should be recognized as a paragraph, list, heading, link, image, multimedia player, form, or one of many other available elements or even a new element that you define.

**Looking to become a front-end web developer?**

We have put together a course that includes all the essential information you need to work towards your goal.

[**Get started**](https://developer.mozilla.org/en-US/docs/Learn/Front-end_web_developer)

### [Prerequisites](https://developer.mozilla.org/en-US/docs/Learn/HTML#prerequisites) <a href="#prerequisites" id="prerequisites"></a>

Before starting this topic, you should have at least basic familiarity with using computers and using the web passively (i.e. just looking at it, consuming the content). You should have a basic work environment set up as detailed in [Installing basic software](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/Installing_basic_software), and understand how to create and manage files, as detailed in [Dealing with files](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/Dealing_with_files) — both are parts of our [Getting started with the web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web) complete beginner's module.

It is recommended that you work through [Getting started with the web ](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web)before attempting this topic. However, this isn't absolutely necessary; much of what is covered in the [HTML basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics) article is also covered in our [Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML) module, albeit in a lot more detail.

After learning HTML, you can then move on to learning about more advanced topics such as:

-   [CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS), and how to use it to style HTML (for example alter your text size and fonts used, add borders and drop shadows, layout your page with multiple columns, add animations and other visual effects.)
-   [JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript), and how to use it to add dynamic functionality to web pages (for example find your location and plot it on a map, make UI elements appear/disappear when you toggle a button, save users' data locally on their computers, and much more.)

### [Modules](https://developer.mozilla.org/en-US/docs/Learn/HTML#modules) <a href="#modules" id="modules"></a>

This topic contains the following modules, in a suggested order for working through them. You should definitely start with the first one.

[Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)

This module sets the stage, getting you used to important concepts and syntax, looking at applying HTML to text, how to create hyperlinks, and how to use HTML to structure a webpage.

[Multimedia and embedding](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding)

This module explores how to use HTML to include multimedia in your web pages, including the different ways that images can be included, and how to embed video, audio, and even entire other webpages.

[HTML tables](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables)

Representing tabular data on a webpage in an understandable, [accessible](https://developer.mozilla.org/en-US/docs/Glossary/Accessibility) way can be a challenge. This module covers basic table markup, along with more complex features such as implementing captions and summaries.

### [Solving common HTML problems](https://developer.mozilla.org/en-US/docs/Learn/HTML#solving_common_html_problems) <a href="#solving_common_html_problems" id="solving_common_html_problems"></a>

[Use HTML to solve common problems](https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto) provides links to sections of content explaining how to use HTML to solve very common problems when creating a webpage: dealing with titles, adding images or videos, emphasizing content, creating a basic form, etc.

### [See also](https://developer.mozilla.org/en-US/docs/Learn/HTML#see_also) <a href="#see_also" id="see_also"></a>

[Web forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)

This module provides a series of articles that will help you master the essentials of web forms. Web forms are a very powerful tool for interacting with users — most commonly they are used for collecting data from users, or allowing them to control a user interface. However, for historical and technical reasons it's not always obvious how to use them to their full potential. We'll cover all the essential aspects of Web forms including marking up their HTML structure, styling form controls, validating form data, and submitting data to the server.

[HTML (HyperText Markup Language)](https://developer.mozilla.org/en-US/docs/Web/HTML)

The main entry point for HTML reference documentation on MDN, including detailed element and attribute references — if you want to know what attributes an element has or what values an attribute has, for example, this is a great place to start.

\\

## What’s in the head? Metadata in HTML

-   [Previous](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)
-   [Overview: Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)
-   [Next](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals)

The [head](https://developer.mozilla.org/en-US/docs/Glossary/Head) of an HTML document is the part that is not displayed in the web browser when the page is loaded. It contains information such as the page [`<title>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title), links to [CSS](https://developer.mozilla.org/en-US/docs/Glossary/CSS) (if you choose to style your HTML content with CSS), links to custom favicons, and other metadata (data about the HTML, such as the author, and important keywords that describe the document.) In this article we'll cover all of the above and more, in order to give you a good basis for working with markup.

| Prerequisites: | Basic HTML familiarity, as covered in [Getting started with HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started). |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Objective:     | To learn about the HTML head, its purpose, the most important items it can contain, and what effect it can have on the HTML document.                        |

### [What is the HTML head?](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#what_is_the_html_head) <a href="#what_is_the_html_head" id="what_is_the_html_head"></a>

Let's revisit the simple [HTML document we covered in the previous article](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started#anatomy_of_an_html_document):

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    <p>This is my page</p>
  </body>
</html>
```

Copy to Clipboard

The HTML head is the contents of the [`<head>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head) element — unlike the contents of the [`<body>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body) element (which are displayed on the page when loaded in a browser), the head's content is not displayed on the page. Instead, the head's job is to contain [metadata](https://developer.mozilla.org/en-US/docs/Glossary/Metadata) about the document. In the above example, the head is quite small:

```
<head>
  <meta charset="utf-8">
  <title>My test page</title>
</head>
```

Copy to Clipboard

In larger pages however, the head can get quite full. Try going to some of your favorite websites and use the [developer tools](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools) to check out their head contents. Our aim here is not to show you how to use everything that can possibly be put in the head, but rather to teach you how to use the major elements that you'll want to include in the head, and give you some familiarity. Let's get started.

### [Adding a title](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#adding_a_title) <a href="#adding_a_title" id="adding_a_title"></a>

We've already seen the [`<title>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title) element in action — this can be used to add a title to the document. This however can get confused with the [`<h1>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements) element, which is used to add a top level heading to your body content — this is also sometimes referred to as the page title. But they are different things!

-   The [`<h1>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements) element appears on the page when loaded in the browser — generally this should be used once per page, to mark up the title of your page content (the story title, or news headline, or whatever is appropriate to your usage.)
-   The [`<title>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title) element is metadata that represents the title of the overall HTML document (not the document's content.)

#### [Active learning: Inspecting a simple example](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#active_learning_inspecting_a_simple_example) <a href="#active_learning_inspecting_a_simple_example" id="active_learning_inspecting_a_simple_example"></a>

1. To start off this active learning, we'd like you to go to our GitHub repo and download a copy of our [title-example.html page](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/the-html-head/title-example.html). To do this, either
    1. Copy and paste the code out of the page and into a new text file in your code editor, then save it in a sensible place.
    2. Press the "Raw" button on the GitHub page, which causes the raw code to appear (possibly in a new browser tab). Next, choose your browser's _File > Save Page As..._ menu and choose a sensible place to save the file.
2. Now open the file in your browser. You should see something like this: ![A simple web page with the title set to <title> element, and the <h1> set to <h1> element.](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML/title-example.png)It should now be completely obvious where the `<h1>` content appears, and where the `<title>` content appears!
3. You should also try opening the code up in your code editor, editing the contents of these elements, then refreshing the page in your browser. Have some fun with it.

The `<title>` element contents are also used in other ways. For example, if you try bookmarking the page (_Bookmarks > Bookmark This Page_ or the star icon in the URL bar in Firefox), you will see the `<title>` contents filled in as the suggested bookmark name.

![A webpage being bookmarked in firefox; the bookmark name has been automatically filled in with the contents of the <title> element](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML/bookmark-example.png)

The `<title>` contents are also used in search results, as you'll see below.

### [Metadata: the \<meta> element](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#metadata_the_meta_element) <a href="#metadata_the_meta_element" id="metadata_the_meta_element"></a>

Metadata is data that describes data, and HTML has an "official" way of adding metadata to a document — the [`<meta>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta) element. Of course, the other stuff we are talking about in this article could also be thought of as metadata too. There are a lot of different types of `<meta>` elements that can be included in your page's \<head>, but we won't try to explain them all at this stage, as it would just get too confusing. Instead, we'll explain a few things that you might commonly see, just to give you an idea.

#### [Specifying your document's character encoding](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#specifying_your_documents_character_encoding) <a href="#specifying_your_documents_character_encoding" id="specifying_your_documents_character_encoding"></a>

In the example we saw above, this line was included:

```
<meta charset="utf-8">
```

Copy to Clipboard

This element specifies the document's character encoding — the character set that the document is permitted to use. `utf-8` is a universal character set that includes pretty much any character from any human language. This means that your web page will be able to handle displaying any language; it's therefore a good idea to set this on every web page you create! For example, your page could handle English and Japanese just fine:

![a web page containing English and Japanese characters, with the character encoding set to universal, or utf-8. Both languages display fine,](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML/correct-encoding.png)If you set your character encoding to `ISO-8859-1`, for example (the character set for the Latin alphabet), your page rendering may appear all messed up:

![a web page containing English and Japanese characters, with the character encoding set to latin. The Japanese characters don't display correctly](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML/bad-encoding.png)

**Note:** Some browsers (like Chrome) automatically fix incorrect encodings, so depending on what browser you use, you may not see this problem. You should still set an encoding of `utf-8` on your page anyway to avoid any potential problems in other browsers.

#### [Active learning: Experiment with character encoding](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#active_learning_experiment_with_character_encoding) <a href="#active_learning_experiment_with_character_encoding" id="active_learning_experiment_with_character_encoding"></a>

To try this out, revisit the simple HTML template you obtained in the previous section on `<title>` (the [title-example.html page](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/the-html-head/title-example.html)), try changing the meta charset value to `ISO-8859-1`, and add the Japanese to your page. This is the code we used:

```
<p>Japanese example: ご飯が熱い。</p>
```

Copy to Clipboard

#### [Adding an author and description](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#adding_an_author_and_description) <a href="#adding_an_author_and_description" id="adding_an_author_and_description"></a>

Many `<meta>` elements include `name` and `content` attributes:

-   `name` specifies the type of meta element it is; what type of information it contains.
-   `content` specifies the actual meta content.

Two such meta elements that are useful to include on your page define the author of the page, and provide a concise description of the page. Let's look at an example:

```
<meta name="author" content="Chris Mills">
<meta name="description" content="The MDN Web Docs Learning Area aims to provide
complete beginners to the Web with all they need to know to get
started with developing web sites and applications.">
```

Copy to Clipboard

Specifying an author is beneficial in many ways: it is useful to be able to understand who wrote the page, if you have any questions about the content and you would like to contact them. Some content management systems have facilities to automatically extract page author information and make it available for such purposes.

Specifying a description that includes keywords relating to the content of your page is useful as it has the potential to make your page appear higher in relevant searches performed in search engines (such activities are termed [Search Engine Optimization](https://developer.mozilla.org/en-US/docs/Glossary/SEO), or [SEO](https://developer.mozilla.org/en-US/docs/Glossary/SEO).)

#### [Active learning: The description's use in search engines](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#active_learning_the_descriptions_use_in_search_engines) <a href="#active_learning_the_descriptions_use_in_search_engines" id="active_learning_the_descriptions_use_in_search_engines"></a>

The description is also used on search engine result pages. Let's go through an exercise to explore this

1. Go to the [front page of The Mozilla Developer Network](https://developer.mozilla.org/en-US/).
2. View the page's source (right-click on the page, choose _View Page Source_ from the context menu.)
3. Find the description meta tag. It will look something like this (although it may change over time):

    ```
    <meta name="description" content="The MDN Web Docs site
      provides information about Open Web technologies
      including HTML, CSS, and APIs for both Web sites and
      progressive web apps.">
    ```

    Copy to Clipboard

4. Now search for "MDN Web Docs" in your favorite search engine (We used Google.) You'll notice the description `<meta>` and `<title>` element content used in the search result — definitely worth having! ![A Yahoo search result for "Mozilla Developer Network"](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML/mdn-search-result.png)

**Note:** In Google, you will see some relevant subpages of MDN Web Docs listed below the main homepage link — these are called sitelinks, and are configurable in [Google's webmaster tools](https://www.google.com/webmasters/tools/) — a way to make your site's search results better in the Google search engine.

**Note:** Many `<meta>` features just aren't used any more. For example, the keyword `<meta>` element (`<meta name="keywords" content="fill, in, your, keywords, here">`) — which is supposed to provide keywords for search engines to determine relevance of that page for different search terms — is ignored by search engines, because spammers were just filling the keyword list with hundreds of keywords, biasing results.

#### [Other types of metadata](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#other_types_of_metadata) <a href="#other_types_of_metadata" id="other_types_of_metadata"></a>

As you travel around the web, you'll find other types of metadata, too. A lot of the features you'll see on websites are proprietary creations, designed to provide certain sites (such as social networking sites) with specific pieces of information they can use.

For example, [Open Graph Data](https://ogp.me) is a metadata protocol that Facebook invented to provide richer metadata for websites. In the MDN Web Docs sourcecode, you'll find this:

```
<meta property="og:image" content="https://developer.mozilla.org/static/img/opengraph-logo.png">
<meta property="og:description" content="The Mozilla Developer Network (MDN) provides
information about Open Web technologies including HTML, CSS, and APIs for both Web sites
and HTML5 Apps. It also documents Mozilla products, like Firefox OS.">
<meta property="og:title" content="Mozilla Developer Network">
```

Copy to Clipboard

One effect of this is that when you link to MDN Web Docs on facebook, the link appears along with an image and description: a richer experience for users.

![Open graph protocol data from the MDN homepage as displayed on facebook, showing an image, title, and description.](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML/facebook-output.png)

Twitter also has its own similar proprietary metadata called [Twitter Cards](https://developer.twitter.com/en/docs/tweets/optimize-with-cards/overview/abouts-cards), which has a similar effect when the site's URL is displayed on twitter.com. For example:

```
<meta name="twitter:title" content="Mozilla Developer Network">
```

Copy to Clipboard

### [Adding custom icons to your site](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#adding_custom_icons_to_your_site) <a href="#adding_custom_icons_to_your_site" id="adding_custom_icons_to_your_site"></a>

To further enrich your site design, you can add references to custom icons in your metadata, and these will be displayed in certain contexts. The most commonly used of these is the **favicon** (short for "favorites icon", referring to its use in the "favorites" or "bookmarks" lists in browsers).

The humble favicon has been around for many years. It is the first icon of this type: a 16-pixel square icon used in multiple places. You may see (depending on the browser) favicons displayed in the browser tab containing each open page, and next to bookmarked pages in the bookmarks panel.

A favicon can be added to your page by:

1. Saving it in the same directory as the site's index page, saved in `.ico` format (most browsers will support favicons in more common formats like `.gif` or `.png`, but using the ICO format will ensure it works as far back as Internet Explorer 6.)
2. Adding the following line into your HTML's [`<head>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head) block to reference it:

    ```
    <link rel="icon" href="favicon.ico" type="image/x-icon">
    ```

    Copy to Clipboard

Here is an example of a favicon in a bookmarks panel:

![The Firefox bookmarks panel, showing a bookmarked example with a favicon displayed next to it.](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML/bookmark-favicon.png)

There are lots of other icon types to consider these days as well. For example, you'll find this in the source code of the MDN Web Docs homepage:

```
<!-- third-generation iPad with high-resolution Retina display: -->
<link rel="apple-touch-icon-precomposed" sizes="144x144" href="https://developer.mozilla.org/static/img/favicon144.png">
<!-- iPhone with high-resolution Retina display: -->
<link rel="apple-touch-icon-precomposed" sizes="114x114" href="https://developer.mozilla.org/static/img/favicon114.png">
<!-- first- and second-generation iPad: -->
<link rel="apple-touch-icon-precomposed" sizes="72x72" href="https://developer.mozilla.org/static/img/favicon72.png">
<!-- non-Retina iPhone, iPod Touch, and Android 2.1+ devices: -->
<link rel="apple-touch-icon-precomposed" href="https://developer.mozilla.org/static/img/favicon57.png">
<!-- basic favicon -->
<link rel="icon" href="https://developer.mozilla.org/static/img/favicon32.png">
```

Copy to Clipboard

The comments explain what each icon is used for — these elements cover things like providing a nice high resolution icon to use when the website is saved to an iPad's home screen.

Don't worry too much about implementing all these types of icon right now — this is a fairly advanced feature, and you won't be expected to have knowledge of this to progress through the course. The main purpose here is to let you know what such things are, in case you come across them while browsing other websites' source code.

**Note:** If your site uses a Content Security Policy (CSP) to enhance its security, the policy applies to the favicon. If you encounter problems with the favicon not loading, verify that the [`Content-Security-Policy`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy) header's [`img-src` directive](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy/img-src) is not preventing access to it.

### [Applying CSS and JavaScript to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#applying_css_and_javascript_to_html) <a href="#applying_css_and_javascript_to_html" id="applying_css_and_javascript_to_html"></a>

Just about all websites you'll use in the modern day will employ [CSS](https://developer.mozilla.org/en-US/docs/Glossary/CSS) to make them look cool, and [JavaScript](https://developer.mozilla.org/en-US/docs/Glossary/JavaScript) to power interactive functionality, such as video players, maps, games, and more. These are most commonly applied to a web page using the [`<link>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link) element and the [`<script>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script) element, respectively.

-   The [`<link>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link) element should always go inside the head of your document. This takes two attributes, `rel="stylesheet"`, which indicates that it is the document's stylesheet, and `href`, which contains the path to the stylesheet file:

    ```
    <link rel="stylesheet" href="my-css-file.css">
    ```

    Copy to Clipboard

-   The [`<script>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script) element should also go into the head, and should include a `src` attribute containing the path to the JavaScript you want to load, and `defer`, which basically instructs the browser to load the JavaScript after the page has finished parsing the HTML. This is useful as it makes sure that the HTML is all loaded before the JavaScript runs, so that you don't get errors resulting from JavaScript trying to access an HTML element that doesn't exist on the page yet. There are actually a number of ways to handle loading JavaScript on your page, but this is the most foolproof one to use for modern browsers (for others, read [Script loading strategies](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript#script_loading_strategies)).

    ```
    <script src="my-js-file.js" defer></script>
    ```

    Copy to Clipboard

    **Note:** The `<script>` element may look like an empty element, but it's not, and so needs a closing tag. Instead of pointing to an external script file, you can also choose to put your script inside the `<script>` element.

#### [Active learning: applying CSS and JavaScript to a page](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#active_learning_applying_css_and_javascript_to_a_page) <a href="#active_learning_applying_css_and_javascript_to_a_page" id="active_learning_applying_css_and_javascript_to_a_page"></a>

1. To start this active learning, grab a copy of our [meta-example.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/the-html-head/meta-example.html), [script.js](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/the-html-head/script.js) and [style.css](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/the-html-head/style.css) files, and save them on your local computer in the same directory. Make sure they are saved with the correct names and file extensions.
2. Open the HTML file in both your browser, and your text editor.
3. By following the information given above, add [`<link>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link) and [`<script>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script) elements to your HTML, so that your CSS and JavaScript are applied to your HTML.

If done correctly, when you save your HTML and refresh your browser you should be able to see that things have changed:

![Example showing a page with CSS and JavaScript applied to it. The CSS has made the page go green, whereas the JavaScript has added a dynamic list to the page.](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML/js-and-css.png)

-   The JavaScript has added an empty list to the page. Now when you click anywhere outside the list, a dialog box will pop up asking you to enter some text for a new list item. When you press the OK button, a new list item will be added to the list containing the text. When you click on an existing list item, a dialog box will pop up allowing you to change the item's text.
-   The CSS has caused the background to go green, and the text to become bigger. It has also styled some of the content that the JavaScript has added to the page (the red bar with the black border is the styling the CSS has added to the JS-generated list.)

**Note:** If you get stuck in this exercise and can't get the CSS/JS to apply, try checking out our [css-and-js.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/the-html-head/css-and-js.html) example page.

### [Setting the primary language of the document](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#setting_the_primary_language_of_the_document) <a href="#setting_the_primary_language_of_the_document" id="setting_the_primary_language_of_the_document"></a>

Finally, it's worth mentioning that you can (and really should) set the language of your page. This can be done by adding the [lang attribute](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/lang) to the opening HTML tag (as seen in the [meta-example.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/the-html-head/meta-example.html) and shown below.)

```
<html lang="en-US">
```

Copy to Clipboard

This is useful in many ways. Your HTML document will be indexed more effectively by search engines if its language is set (allowing it to appear correctly in language-specific results, for example), and it is useful to people with visual impairments using screen readers (for example, the word "six" exists in both French and English, but is pronounced differently.)

You can also set subsections of your document to be recognized as different languages. For example, we could set our Japanese language section to be recognized as Japanese, like so:

```
<p>Japanese example: <span lang="ja">ご飯が熱い。</span>.</p>
```

Copy to Clipboard

These codes are defined by the [ISO 639-1](https://en.wikipedia.org/wiki/ISO_639-1) standard. You can find more about them in [Language tags in HTML and XML](https://www.w3.org/International/articles/language-tags/).

### [Summary](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#summary) <a href="#summary" id="summary"></a>

That marks the end of our quickfire tour of the HTML head — there's a lot more you can do in here, but an exhaustive tour would be boring and confusing at this stage, and we just wanted to give you an idea of the most common things you'll find in there for now! In the next article we'll be looking at HTML text

One of HTML's main jobs is to give text structure so that a browser can display an HTML document the way its developer intends. This article explains the way [HTML](https://developer.mozilla.org/en-US/docs/Glossary/HTML) can be used to structure a page of text by adding headings and paragraphs, emphasizing words, creating lists, and more.

| Prerequisites: | Basic HTML familiarity, as covered in [Getting started with HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started). |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Objective:     | Learn how to mark up a basic page of text to give it structure and meaning—including paragraphs, headings, lists, emphasis, and quotations.                  |

### [The basics: headings and paragraphs](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#the_basics_headings_and_paragraphs) <a href="#the_basics_headings_and_paragraphs" id="the_basics_headings_and_paragraphs"></a>

Most structured text consists of headings and paragraphs, whether you are reading a story, a newspaper, a college textbook, a magazine, etc.

![An example of a newspaper front cover, showing use of a top level heading, subheadings and paragraphs.](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals/newspaper_small.jpg)

Structured content makes the reading experience easier and more enjoyable.

In HTML, each paragraph has to be wrapped in a [`<p>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p) element, like so:

```
<p>I am a paragraph, oh yes I am.</p>
```

Copy to Clipboard

Each heading has to be wrapped in a heading element:

```
<h1>I am the title of the story.</h1>
```

Copy to Clipboard

There are six heading elements: [`<h1>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements), [`<h2>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements), [`<h3>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements), [`<h4>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements), [`<h5>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements), and [`<h6>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements). Each element represents a different level of content in the document; `<h1>` represents the main heading, `<h2>` represents subheadings, `<h3>` represents sub-subheadings, and so on.

#### [Implementing structural hierarchy](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#implementing_structural_hierarchy) <a href="#implementing_structural_hierarchy" id="implementing_structural_hierarchy"></a>

For example, in this story, the `<h1>` element represents the title of the story, the `<h2>` elements represent the title of each chapter, and the `<h3>` elements represent sub-sections of each chapter:

```
<h1>The Crushing Bore</h1>

<p>By Chris Mills</p>

<h2>Chapter 1: The dark night</h2>

<p>It was a dark night. Somewhere, an owl hooted. The rain lashed down on the ...</p>

<h2>Chapter 2: The eternal silence</h2>

<p>Our protagonist could not so much as a whisper out of the shadowy figure ...</p>

<h3>The specter speaks</h3>

<p>Several more hours had passed, when all of a sudden the specter sat bolt upright and exclaimed, "Please have mercy on my soul!"</p>
```

Copy to Clipboard

It's really up to you what the elements involved represent, as long as the hierarchy makes sense. You just need to bear in mind a few best practices as you create such structures:

-   Preferably, you should use a single `<h1>` per page—this is the top level heading, and all others sit below this in the hierarchy.
-   Make sure you use the headings in the correct order in the hierarchy. Don't use `<h3>` elements to represent subheadings, followed by `<h2>` elements to represent sub-subheadings—that doesn't make sense and will lead to weird results.
-   Of the six heading levels available, you should aim to use no more than three per page, unless you feel it is necessary. Documents with many levels (for example, a deep heading hierarchy) become unwieldy and difficult to navigate. On such occasions, it is advisable to spread the content over multiple pages if possible.

#### [Why do we need structure?](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#why_do_we_need_structure) <a href="#why_do_we_need_structure" id="why_do_we_need_structure"></a>

To answer this question, let's take a look at [text-start.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/html-text-formatting/text-start.html)—the starting point of our running example for this article (a nice hummus recipe). You should save a copy of this file on your local machine, as you'll need it for the exercises later on. This document's body currently contains multiple pieces of content. They aren't marked up in any way, but they are separated with linebreaks (Enter/Return pressed to go onto the next line).

However, when you open the document in your browser, you'll see that the text appears as a big chunk!

![A webpage that shows a wall of unformatted text, because there are no elements on the page to structure it.](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals/screen_shot_2017-03-29_at_09.20.35.png)

This is because there are no elements to give the content structure, so the browser does not know what is a heading and what is a paragraph. Furthermore:

-   Users looking at a web page tend to scan quickly to find relevant content, often just reading the headings, to begin with. (We usually [spend a very short time on a web page](https://www.nngroup.com/articles/how-long-do-users-stay-on-web-pages/).) If they can't see anything useful within a few seconds, they'll likely get frustrated and go somewhere else.
-   Search engines indexing your page consider the contents of headings as important keywords for influencing the page's search rankings. Without headings, your page will perform poorly in terms of [SEO](https://developer.mozilla.org/en-US/docs/Glossary/SEO) (Search Engine Optimization).
-   Severely visually impaired people often don't read web pages; they listen to them instead. This is done with software called a [screen reader](https://en.wikipedia.org/wiki/Screen_reader). This software provides ways to get fast access to given text content. Among the various techniques used, they provide an outline of the document by reading out the headings, allowing their users to find the information they need quickly. If headings are not available, they will be forced to listen to the whole document read out loud.
-   To style content with [CSS](https://developer.mozilla.org/en-US/docs/Glossary/CSS), or make it do interesting things with [JavaScript](https://developer.mozilla.org/en-US/docs/Glossary/JavaScript), you need to have elements wrapping the relevant content, so CSS/JavaScript can effectively target it.

Therefore, we need to give our content structural markup.

#### [Active learning: Giving our content structure](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#active_learning_giving_our_content_structure) <a href="#active_learning_giving_our_content_structure" id="active_learning_giving_our_content_structure"></a>

Let's jump straight in with a live example. In the example below, add elements to the raw text in the _Input_ field so that it appears as a heading and two paragraphs in the _Output_ field.

If you make a mistake, you can always reset it using the _Reset_ button. If you get stuck, press the _Show solution_ button to see the answer.

#### [Why do we need semantics?](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#why_do_we_need_semantics) <a href="#why_do_we_need_semantics" id="why_do_we_need_semantics"></a>

Semantics are relied on everywhere around us—we rely on previous experience to tell us what the function of an everyday object is; when we see something, we know what its function will be. So, for example, we expect a red traffic light to mean "stop," and a green traffic light to mean "go." Things can get tricky very quickly if the wrong semantics are applied. (Do any countries use red to mean "go"? We hope not.)

In a similar vein, we need to make sure we are using the correct elements, giving our content the correct meaning, function, or appearance. In this context, the [`<h1>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements) element is also a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."

```
<h1>This is a top level heading</h1>
```

Copy to Clipboard

By default, the browser will give it a large font size to make it look like a heading (although you could style it to look like anything you wanted using CSS). More importantly, its semantic value will be used in multiple ways, for example by search engines and screen readers (as mentioned above).

On the other hand, you could make any element _look_ like a top level heading. Consider the following:

```
<span style="font-size: 32px; margin: 21px 0; display: block;">Is this a top level heading?</span>
```

Copy to Clipboard

This is a [`<span>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/span) element. It has no semantics. You use it to wrap content when you want to apply CSS to it (or do something to it with JavaScript) without giving it any extra meaning. (You'll find out more about these later on in the course.) We've applied some CSS to it to make it look like a top level heading, but since it has no semantic value, it will not get any of the extra benefits described above. It is a good idea to use the relevant HTML element for the job.

### [Lists](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#lists) <a href="#lists" id="lists"></a>

Now let's turn our attention to lists. Lists are everywhere in life—from your shopping list to the list of directions you subconsciously follow to get to your house every day, to the lists of instructions you are following in these tutorials! Lists are everywhere on the web, too, and we've got three different types to worry about.

#### [Unordered](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#unordered) <a href="#unordered" id="unordered"></a>

Unordered lists are used to mark up lists of items for which the order of the items doesn't matter. Let's take a shopping list as an example:

```
milk
eggs
bread
hummus
```

Every unordered list starts off with a [`<ul>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul) element—this wraps around all the list items:

```
<ul>
milk
eggs
bread
hummus
</ul>
```

Copy to Clipboard

The last step is to wrap each list item in a [`<li>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/li) (list item) element:

```
<ul>
  <li>milk</li>
  <li>eggs</li>
  <li>bread</li>
  <li>hummus</li>
</ul>
```

Copy to Clipboard

**Active learning: Marking up an unordered list**

Try editing the live sample below to create your very own HTML unordered list.

#### [Ordered](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#ordered) <a href="#ordered" id="ordered"></a>

Ordered lists are lists in which the order of the items _does_ matter. Let's take a set of directions as an example:

```
Drive to the end of the road
Turn right
Go straight across the first two roundabouts
Turn left at the third roundabout
The school is on your right, 300 meters up the road
```

The markup structure is the same as for unordered lists, except that you have to wrap the list items in an [`<ol>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol) element, rather than `<ul>`:

```
<ol>
  <li>Drive to the end of the road</li>
  <li>Turn right</li>
  <li>Go straight across the first two roundabouts</li>
  <li>Turn left at the third roundabout</li>
  <li>The school is on your right, 300 meters up the road</li>
</ol>
```

Copy to Clipboard

**Active learning: Marking up an ordered list**

Try editing the live sample below to create your very own HTML ordered list.

#### [Active learning: Marking up our recipe page](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#active_learning_marking_up_our_recipe_page) <a href="#active_learning_marking_up_our_recipe_page" id="active_learning_marking_up_our_recipe_page"></a>

So at this point in the article, you have all the information you need to mark up our recipe page example. You can choose to either save a local copy of our [text-start.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/html-text-formatting/text-start.html) starting file and do the work there or do it in the editable example below. Doing it locally will probably be better, as then you'll get to save the work you are doing, whereas if you fill it in to the editable example, it will be lost the next time you open the page. Both have pros and cons.

If you get stuck, you can always press the _Show solution_ button, or check out our [text-complete.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/html-text-formatting/text-complete.html) example on our github repo.

#### [Nesting lists](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#nesting_lists) <a href="#nesting_lists" id="nesting_lists"></a>

It is perfectly OK to nest one list inside another one. You might want to have some sub-bullets sitting below a top-level bullet. Let's take the second list from our recipe example:

```
<ol>
  <li>Remove the skin from the garlic, and chop coarsely.</li>
  <li>Remove all the seeds and stalk from the pepper, and chop coarsely.</li>
  <li>Add all the ingredients into a food processor.</li>
  <li>Process all the ingredients into a paste.</li>
  <li>If you want a coarse "chunky" hummus, process it for a short time.</li>
  <li>If you want a smooth hummus, process it for a longer time.</li>
</ol>
```

Copy to Clipboard

Since the last two bullets are very closely related to the one before them (they read like sub-instructions or choices that fit below that bullet), it might make sense to nest them inside their own unordered list and put that list inside the current fourth bullet. This would look like so:

```
<ol>
  <li>Remove the skin from the garlic, and chop coarsely.</li>
  <li>Remove all the seeds and stalk from the pepper, and chop coarsely.</li>
  <li>Add all the ingredients into a food processor.</li>
  <li>Process all the ingredients into a paste.
    <ul>
      <li>If you want a coarse "chunky" hummus, process it for a short time.</li>
      <li>If you want a smooth hummus, process it for a longer time.</li>
    </ul>
  </li>
</ol>
```

Copy to Clipboard

Try going back to the previous active learning example and updating the second list like this.

### [Emphasis and importance](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#emphasis_and_importance) <a href="#emphasis_and_importance" id="emphasis_and_importance"></a>

In human language, we often emphasize certain words to alter the meaning of a sentence, and we often want to mark certain words as important or different in some way. HTML provides various semantic elements to allow us to mark up textual content with such effects, and in this section, we'll look at a few of the most common ones.

#### [Emphasis](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#emphasis) <a href="#emphasis" id="emphasis"></a>

When we want to add emphasis in spoken language, we _stress_ certain words, subtly altering the meaning of what we are saying. Similarly, in written language we tend to stress words by putting them in italics. For example, the following two sentences have different meanings.

I am glad you weren't late.

I am _glad_ you weren't _late_.

The first sentence sounds genuinely relieved that the person wasn't late. In contrast, the second one sounds sarcastic or passive-aggressive, expressing annoyance that the person arrived a bit late.

In HTML we use the [`<em>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/em) (emphasis) element to mark up such instances. As well as making the document more interesting to read, these are recognized by screen readers and spoken out in a different tone of voice. Browsers style this as italic by default, but you shouldn't use this tag purely to get italic styling. To do that, you'd use a [`<span>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/span) element and some CSS, or perhaps an [`<i>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/i) element (see below).

```
<p>I am <em>glad</em> you weren't <em>late</em>.</p>
```

Copy to Clipboard

#### [Strong importance](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#strong_importance) <a href="#strong_importance" id="strong_importance"></a>

To emphasize important words, we tend to stress them in spoken language and **bold** them in written language. For example:

This liquid is **highly toxic**.

I am counting on you. **Do not** be late!

In HTML we use the [`<strong>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/strong) (strong importance) element to mark up such instances. As well as making the document more useful, again these are recognized by screen readers and spoken in a different tone of voice. Browsers style this as bold text by default, but you shouldn't use this tag purely to get bold styling. To do that, you'd use a [`<span>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/span) element and some CSS, or perhaps a [`<b>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/b) element (see below).

```
<p>This liquid is <strong>highly toxic</strong>.</p>

<p>I am counting on you. <strong>Do not</strong> be late!</p>
```

Copy to Clipboard

You can nest strong and emphasis inside one another if desired:

```
<p>This liquid is <strong>highly toxic</strong> —
if you drink it, <strong>you may <em>die</em></strong>.</p>
```

Copy to Clipboard

#### [Active learning: Let's be important](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#active_learning_lets_be_important) <a href="#active_learning_lets_be_important" id="active_learning_lets_be_important"></a>

In this active learning section, we've provided an editable example. Inside it, we'd like you to try adding emphasis and strong importance to the words you think need them, just to have some practice.

#### [Italic, bold, underline...](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#italic_bold_underline) <a href="#italic_bold_underline" id="italic_bold_underline"></a>

The elements we've discussed so far have clearcut associated semantics. The situation with [`<b>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/b), [`<i>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/i), and [`<u>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/u) is somewhat more complicated. They came about so people could write bold, italics, or underlined text in an era when CSS was still supported poorly or not at all. Elements like this, which only affect presentation and not semantics, are known as **presentational elements** and should no longer be used because, as we've seen before, semantics is so important to accessibility, SEO, etc.

HTML5 redefined `<b>`, `<i>`, and `<u>` with new, somewhat confusing, semantic roles.

Here's the best rule of thumb: It's likely appropriate to use `<b>`, `<i>`, or `<u>` to convey a meaning traditionally conveyed with bold, italics, or underline, provided there is no more suitable element. However, it always remains critical to keep an accessibility mindset. The concept of italics isn't very helpful to people using screen readers, or to people using a writing system other than the Latin alphabet.

-   [`<i>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/i) is used to convey a meaning traditionally conveyed by italic: foreign words, taxonomic designation, technical terms, a thought...
-   [`<b>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/b) is used to convey a meaning traditionally conveyed by bold: key words, product names, lead sentence...
-   [`<u>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/u) is used to convey a meaning traditionally conveyed by underline: proper name, misspelling...

**Note:** People strongly associate underlining with hyperlinks. Therefore, on the web, it's best to underline only links. Use the `<u>` element when it's semantically appropriate, but consider using CSS to change the default underline to something more appropriate on the web. The example below illustrates how it can be done.

```
<!-- scientific names -->
<p>
  The Ruby-throated Hummingbird (<i>Archilochus colubris</i>)
  is the most common hummingbird in Eastern North America.
</p>

<!-- foreign words -->
<p>
  The menu was a sea of exotic words like <i lang="uk-latn">vatrushka</i>,
  <i lang="id">nasi goreng</i> and <i lang="fr">soupe à l'oignon</i>.
</p>

<!-- a known misspelling -->
<p>
  Someday I'll learn how to <u style="text-decoration-line: underline; text-decoration-style: wavy;">spel</u> better.
</p>

<!-- Highlight keywords in a set of instructions -->
<ol>
  <li>
    <b>Slice</b> two pieces of bread off the loaf.
  </li>
  <li>
    <b>Insert</b> a tomato slice and a leaf of
    lettuce between the slices of bread.
  </li>
</ol>
```

Copy to Clipboard

### [Test your skills!](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#test_your_skills!) <a href="#test_your_skills" id="test_your_skills"></a>

You've reached the end of this article, but can you remember the most important information? You can find some further tests to verify that you've retained this information before you move on—see [Test your skills: HTML text basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Test_your_skills:_HTML_text_basics).

### [Summary](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals#summary) <a href="#summary" id="summary"></a>

That's it for now! This article should have given you a good idea of how to start marking up text in HTML and introduced you to some of the most important elements in this area. There are a lot more semantic elements to cover in this area, and we'll look at a lot more in our [Advanced text formatting](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting) article later on in the course. In the next article, we'll be looking in detail at how to [create hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks), possibly the most important element on the web.Hyperlinks are really important — they are what makes the Web _a web_. This article shows the syntax required to make a link, and discusses link best practices.

| Prerequisites: | Basic HTML familiarity, as covered in [Getting started with HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started). HTML text formatting, as covered in [HTML text fundamentals](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals). |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Objective:     | To learn how to implement a hyperlink effectively, and link multiple files together.                                                                                                                                                                                                                                        |

### [What is a hyperlink?](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#what_is_a_hyperlink) <a href="#what_is_a_hyperlink" id="what_is_a_hyperlink"></a>

Hyperlinks are one of the most exciting innovations the Web has to offer. They've been a feature of the Web since the beginning, and are what makes the Web _a web._ Hyperlinks allow us to link documents to other documents or resources, link to specific parts of documents, or make apps available at a web address. Almost any web content can be converted to a link so that when clicked or otherwise activated the web browser goes to another web address ([URL](https://developer.mozilla.org/en-US/docs/Glossary/URL)).

**Note:** A URL can point to HTML files, text files, images, text documents, video and audio files, or anything else that lives on the Web. If the web browser doesn't know how to display or handle the file, it will ask you if you want to open the file (in which case the duty of opening or handling the file is passed to a suitable native app on the device) or download the file (in which case you can try to deal with it later on).

For example, the BBC homepage contains many links that point not only to multiple news stories, but also different areas of the site (navigation functionality), login/registration pages (user tools), and more.

![frontpage of bbc.co.uk, showing many news items, and navigation menu functionality](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks/updated-bbc-website.png)

### [Anatomy of a link](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#anatomy_of_a_link) <a href="#anatomy_of_a_link" id="anatomy_of_a_link"></a>

A basic link is created by wrapping the text or other content, see [Block level links](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#block_level_links), inside an [`<a>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a) element and using the [`href`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a#attr-href) attribute, also known as a **Hypertext Reference**, or **target**, that contains the web address.

```
<p>I'm creating a link to
<a href="https://www.mozilla.org/en-US/">the Mozilla homepage</a>.
</p>
```

Copy to Clipboard

This gives us the following result:

I'm creating a link to [the Mozilla homepage](https://www.mozilla.org/en-US/).

#### [Adding supporting information with the title attribute](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#adding_supporting_information_with_the_title_attribute) <a href="#adding_supporting_information_with_the_title_attribute" id="adding_supporting_information_with_the_title_attribute"></a>

Another attribute you may want to add to your links is `title`. The title contains additional information about the link, such as which kind of information the page contains, or things to be aware of on the web site.

```
<p>I'm creating a link to
<a href="https://www.mozilla.org/en-US/"
   title="The best place to find more information about Mozilla's
          mission and how to contribute">the Mozilla homepage</a>.
</p>
```

Copy to Clipboard

This gives us the following result and hovering over the link displays the title as a tooltip:

I'm creating a link to [the Mozilla homepage](https://www.mozilla.org/en-US/).

**Note:** A link title is only revealed on mouse hover, which means that people relying on keyboard controls or touchscreens to navigate web pages will have difficulty accessing title information. If a title's information is truly important to the usability of the page, then you should present it in a manner that will be accessible to all users, for example by putting it in the regular text.

#### [Active learning: creating your own example link](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#active_learning_creating_your_own_example_link) <a href="#active_learning_creating_your_own_example_link" id="active_learning_creating_your_own_example_link"></a>

Create an HTML document using your local code editor and our [getting started template](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/getting-started/index.html).

-   Inside the HTML body, add one or more paragraphs or other types of content you already know about.
-   Change some of the content into links.
-   Include title attributes.

#### [Block level links](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#block_level_links) <a href="#block_level_links" id="block_level_links"></a>

As mentioned before, almost any content can be made into a link, even [block-level elements](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started#block_versus_inline_elements). If you have an image you want to make into a link, use the [`<a>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a) element and reference the image file with the [`<img>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img) element.

```
<a href="https://www.mozilla.org/en-US/">
  <img src="mozilla-image.png" alt="mozilla logo that links to the mozilla homepage">
</a>
```

Copy to Clipboard

**Note:** You'll find out more about using images on the Web in a future article.

### [A quick primer on URLs and paths](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#a_quick_primer_on_urls_and_paths) <a href="#a_quick_primer_on_urls_and_paths" id="a_quick_primer_on_urls_and_paths"></a>

To fully understand link targets, you need to understand URLs and file paths. This section gives you the information you need to achieve this.

A URL, or Uniform Resource Locator is a string of text that defines where something is located on the Web. For example, Mozilla's English homepage is located at `https://www.mozilla.org/en-US/`.

URLs use paths to find files. Paths specify where the file you're interested in is located in the filesystem. Let's look at an example of a directory structure, see the [creating-hyperlinks](https://github.com/mdn/learning-area/tree/master/html/introduction-to-html/creating-hyperlinks) directory.

![A simple directory structure. The parent directory is called creating-hyperlinks and contains two files called index.html and contacts.html, and two directories called projects and pdfs, which contain an index.html and a project-brief.pdf file, respectively](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks/simple-directory.png)

The **root** of this directory structure is called `creating-hyperlinks`. When working locally with a web site, you'll have one directory that contains the entire site. Inside the **root**, we have an `index.html` file and a `contacts.html`. In a real website, `index.html` would be our home page or landing page (a web page that serves as the entry point for a website or a particular section of a website.).

There are also two directories inside our root — `pdfs` and `projects`. These each have a single file inside them — a PDF (`project-brief.pdf`) and an `index.html` file, respectively. Note that you can have two `index.html` files in one project, as long as they're in different filesystem locations. The second `index.html` would perhaps be the main landing page for project-related information.

-   **Same directory**: If you wanted to include a hyperlink inside `index.html` (the top level `index.html`) pointing to `contacts.html`, you would specify the filename that you want to link to, because it's in the same directory as the current file. The URL you would use is `contacts.html`:

    ```
    <p>Want to contact a specific staff member?
    Find details on our <a href="contacts.html">contacts page</a>.</p>
    ```

    Copy to Clipboard

-   **Moving down into subdirectories**: If you wanted to include a hyperlink inside `index.html` (the top level `index.html`) pointing to `projects/index.html`, you would need to go down into the `projects` directory before indicating the file you want to link to. This is done by specifying the directory's name, then a forward slash, then the name of the file. The URL you would use is `projects/index.html`:

    ```
    <p>Visit my <a href="projects/index.html">project homepage</a>.</p>
    ```

    Copy to Clipboard

-   **Moving back up into parent directories**: If you wanted to include a hyperlink inside `projects/index.html` pointing to `pdfs/project-brief.pdf`, you'd have to go up a directory level, then back down into the `pdf` directory. To go up a directory, use two dots — `..` — so the URL you would use is `../pdfs/project-brief.pdf`:

    ```
    <p>A link to my <a href="../pdfs/project-brief.pdf">project brief</a>.</p>
    ```

    Copy to Clipboard

**Note:** You can combine multiple instances of these features into complex URLs, if needed, for example: `../../../complex/path/to/my/file.html`.

#### [Document fragments](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#document_fragments) <a href="#document_fragments" id="document_fragments"></a>

It's possible to link to a specific part of an HTML document, known as a **document fragment**, rather than just to the top of the document. To do this you first have to assign an [`id`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes#attr-id) attribute to the element you want to link to. It normally makes sense to link to a specific heading, so this would look something like the following:

```
<h2 id="Mailing_address">Mailing address</h2>
```

Copy to Clipboard

Then to link to that specific `id`, you'd include it at the end of the URL, preceded by a hash/pound symbol (`#`), for example:

```
<p>Want to write us a letter? Use our <a href="contacts.html#Mailing_address">mailing address</a>.</p>
```

Copy to Clipboard

You can even use the document fragment reference on its own to link to _another part of the current document_:

```
<p>The <a href="#Mailing_address">company mailing address</a> can be found at the bottom of this page.</p>
```

Copy to Clipboard

#### [Absolute versus relative URLs](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#absolute_versus_relative_urls) <a href="#absolute_versus_relative_urls" id="absolute_versus_relative_urls"></a>

Two terms you'll come across on the Web are **absolute URL** and **relative URL:**

**absolute URL**: Points to a location defined by its absolute location on the web, including [protocol](https://developer.mozilla.org/en-US/docs/Glossary/Protocol) and [domain name](https://developer.mozilla.org/en-US/docs/Glossary/Domain_name). For example, if an `index.html` page is uploaded to a directory called `projects` that sits inside the **root** of a web server, and the web site's domain is `https://www.example.com`, the page would be available at `https://www.example.com/projects/index.html` (or even just `https://www.example.com/projects/`, as most web servers just look for a landing page such as `index.html` to load if it isn't specified in the URL.)

An absolute URL will always point to the same location, no matter where it's used.

**relative URL**: Points to a location that is _relative_ to the file you are linking from, more like what we looked at in the previous section. For example, if we wanted to link from our example file at `https://www.example.com/projects/index.html` to a PDF file in the same directory, the URL would just be the filename — `project-brief.pdf` — no extra information needed. If the PDF was available in a subdirectory inside `projects` called `pdfs`, the relative link would be `pdfs/project-brief.pdf` (the equivalent absolute URL would be `https://www.example.com/projects/pdfs/project-brief.pdf`.)

A relative URL will point to different places depending on the actual location of the file you refer from — for example if we moved our `index.html` file out of the `projects` directory and into the **root** of the web site (the top level, not in any directories), the `pdfs/project-brief.pdf` relative URL link inside it would now point to a file located at `https://www.example.com/pdfs/project-brief.pdf`, not a file located at `https://www.example.com/projects/pdfs/project-brief.pdf`.

Of course, the location of the `project-brief.pdf` file and `pdfs` folder won't suddenly change because you moved the `index.html` file — this would make your link point to the wrong place, so it wouldn't work if clicked on. You need to be careful!

### [Link best practices](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#link_best_practices) <a href="#link_best_practices" id="link_best_practices"></a>

There are some best practices to follow when writing links. Let's look at these now.

#### [Use clear link wording](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#use_clear_link_wording) <a href="#use_clear_link_wording" id="use_clear_link_wording"></a>

It's easy to throw links up on your page. That's not enough. We need to make our links _accessible_ to all readers, regardless of their current context and which tools they prefer. For example:

-   Screenreader users like jumping around from link to link on the page, and reading links out of context.
-   Search engines use link text to index target files, so it is a good idea to include keywords in your link text to effectively describe what is being linked to.
-   Visual readers skim over the page rather than reading every word, and their eyes will be drawn to page features that stand out, like links. They will find descriptive link text useful.

Let's look at a specific example:

**Good** link text: [Download Firefox](https://firefox.com)

```
<p><a href="https://firefox.com/">
  Download Firefox
</a></p>
```

Copy to Clipboard

**Bad** link text: [Click here](https://firefox.com) to download Firefox

```
<p><a href="https://firefox.com/">
  Click here
</a>
to download Firefox</p>
```

Copy to Clipboard

Other tips:

-   Don't repeat the URL as part of the link text — URLs look ugly, and sound even uglier when a screen reader reads them out letter by letter.
-   Don't say "link" or "links to" in the link text — it's just noise. Screen readers tell people there's a link. Visual users will also know there's a link, because links are generally styled in a different color and underlined (this convention generally shouldn't be broken, as users are used to it).
-   Keep your link text as short as possible — this is helpful because screen readers need to interpret the entire link text.
-   Minimize instances where multiple copies of the same text are linked to different places. This can cause problems for screen reader users, if there's a list of links out of context that are labeled "click here", "click here", "click here".

#### [Linking to non-HTML resources — leave clear signposts](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#linking_to_non-html_resources_%E2%80%94_leave_clear_signposts) <a href="#linking_to_non-html_resources_-_leave_clear_signposts" id="linking_to_non-html_resources_-_leave_clear_signposts"></a>

When linking to a resource that will be downloaded (like a PDF or Word document), streamed (like video or audio), or has another potentially unexpected effect (opens a popup window, or loads a Flash movie), you should add clear wording to reduce any confusion.

For example:

-   If you're on a low bandwidth connection, click a link, and then a multiple megabyte download starts unexpectedly.
-   If you don't have the Flash player installed, click a link, and then suddenly get taken to a page that requires Flash.

Let's look at some examples, to see what kind of text can be used here:

```
<p><a href="https://www.example.com/large-report.pdf">
  Download the sales report (PDF, 10MB)
</a></p>

<p><a href="https://www.example.com/video-stream/" target="_blank">
  Watch the video (stream opens in separate tab, HD quality)
</a></p>

<p><a href="https://www.example.com/car-game">
  Play the car game (requires Flash)
</a></p>
```

Copy to Clipboard

#### [Use the download attribute when linking to a download](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#use_the_download_attribute_when_linking_to_a_download) <a href="#use_the_download_attribute_when_linking_to_a_download" id="use_the_download_attribute_when_linking_to_a_download"></a>

When you are linking to a resource that's to be downloaded rather than opened in the browser, you can use the `download` attribute to provide a default save filename. Here's an example with a download link to the latest Windows version of Firefox:

```
<a href="https://download.mozilla.org/?product=firefox-latest-ssl&os=win64&lang=en-US"
   download="firefox-latest-64bit-installer.exe">
  Download Latest Firefox for Windows (64-bit) (English, US)
</a>
```

Copy to Clipboard

### [Active learning: creating a navigation menu](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#active_learning_creating_a_navigation_menu) <a href="#active_learning_creating_a_navigation_menu" id="active_learning_creating_a_navigation_menu"></a>

For this exercise, we'd like you to link some pages together with a navigation menu to create a multi-page website. This is one common way in which a website is created — the same page structure is used on every page, including the same navigation menu, so when links are clicked it gives the impression that you are staying in the same place, and different content is being brought up.

You'll need to make local copies of the following four pages, all in the same directory. For a complete file list, see the [navigation-menu-start](https://github.com/mdn/learning-area/tree/master/html/introduction-to-html/navigation-menu-start) directory:

-   [index.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/navigation-menu-start/index.html)
-   [projects.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/navigation-menu-start/projects.html)
-   [pictures.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/navigation-menu-start/pictures.html)
-   [social.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/navigation-menu-start/social.html)

You should:

1. Add an unordered list in the indicated place on one page that includes the names of the pages to link to. A navigation menu is usually just a list of links, so this is semantically OK.
2. Change each page name into a link to that page.
3. Copy the navigation menu across to each page.
4. On each page, remove just the link to that same page — it's confusing and unnecessary for a page to include a link to itself. And, the lack of a link acts a good visual reminder of which page you are currently on.

The finished example should look similar to the following page:

![An example of a simple HTML navigation menu, with home, pictures, projects, and social menu items](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks/navigation-example.png)

**Note:** If you get stuck, or aren't sure if you have got it right, you can check the [navigation-menu-marked-up](https://github.com/mdn/learning-area/tree/master/html/introduction-to-html/navigation-menu-marked-up) directory to see the correct answer.

### [E-mail links](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#e-mail_links) <a href="#e-mail_links" id="e-mail_links"></a>

It's possible to create links or buttons that, when clicked, open a new outgoing email message rather than linking to a resource or page. This is done using the [`<a>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a) element and the `mailto:` URL scheme.

In its most basic and commonly used form, a `mailto:` link indicates the email address of the intended recipient. For example:

```
<a href="mailto:nowhere@mozilla.org">Send email to nowhere</a>
```

Copy to Clipboard

This results in a link that looks like this: [Send email to nowhere](mailto:nowhere@mozilla.org).

In fact, the email address is optional. If you omit it and your [`href`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a#attr-href) is "mailto:", a new outgoing email window will be opened by the user's email client with no destination address. This is often useful as "Share" links that users can click to send an email to an address of their choosing.

#### [Specifying details](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#specifying_details) <a href="#specifying_details" id="specifying_details"></a>

In addition to the email address, you can provide other information. In fact, any standard mail header fields can be added to the `mailto` URL you provide. The most commonly used of these are "subject", "cc", and "body" (which is not a true header field, but allows you to specify a short content message for the new email). Each field and its value is specified as a query term.

Here's an example that includes a cc, bcc, subject and body:

```
<a href="mailto:nowhere@mozilla.org?cc=name2@rapidtables.com&bcc=name3@rapidtables.com&subject=The%20subject%20of%20the%20email&body=The%20body%20of%20the%20email">
  Send mail with cc, bcc, subject and body
</a>
```

Copy to Clipboard

**Note:** The values of each field must be URL-encoded, that is with non-printing characters (invisible characters like tabs, carriage returns, and page breaks) and spaces [percent-escaped](https://en.wikipedia.org/wiki/Percent-encoding). Also, note the use of the question mark (`?`) to separate the main URL from the field values, and ampersands (&) to separate each field in the `mailto:` URL. This is standard URL query notation. Read [The GET method](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data#the_get_method) to understand what URL query notation is more commonly used for.

Here are a few other sample `mailto` URLs:

-   [mailto:](mailto:)
-   [mailto:nowhere@mozilla.org](mailto:nowhere@mozilla.org)
-   [mailto:nowhere@mozilla.org,nobody@mozilla.org](mailto:nowhere@mozilla.org,nobody@mozilla.org)
-   [mailto:nowhere@mozilla.org?cc=nobody@mozilla.org](mailto:nowhere@mozilla.org?cc=nobody@mozilla.org)
-   [mailto:nowhere@mozilla.org?cc=nobody@mozilla.org\&subject=This%20is%20the%20subject](mailto:nowhere@mozilla.org?cc=nobody@mozilla.org&subject=This%20is%20the%20subject)

### [Test your skills!](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#test_your_skills!) <a href="#test_your_skills" id="test_your_skills"></a>

You've reached the end of this article, but can you remember the most important information? You can find some further tests to verify that you've retained this information before you move on — see [Test your skills: Links](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Test_your_skills:_Links).

### [Summary](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#summary) <a href="#summary" id="summary"></a>

That's it for links, for now anyway! You'll return to links later on in the course when you start to look at styling them. Next up for HTML, we'll return to text semantics and look at some more advanced/unusual features that you'll find useful — Advanced text formatting is your next stop.

There are many other elements in HTML for formatting text, which we didn't get to in the [HTML text fundamentals](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals) article. The elements described in this article are less known, but still useful to know about (and this is still not a complete list by any means). Here you'll learn about marking up quotations, description lists, computer code and other related text, subscript and superscript, contact information, and more.

| Prerequisites: | Basic HTML familiarity, as covered in [Getting started with HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started). HTML text formatting, as covered in [HTML text fundamentals](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals). |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Objective:     | To learn how to use lesser-known HTML elements to mark up advanced semantic features.                                                                                                                                                                                                                                       |

### [Description lists](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#description_lists) <a href="#description_lists" id="description_lists"></a>

In HTML text fundamentals, we walked through how to [mark up basic lists](https://developer.mozilla.org/en-US/docs/Learn/HTML#lists) in HTML, but we didn't mention the third type of list you'll occasionally come across — **description lists**. The purpose of these lists is to mark up a set of items and their associated descriptions, such as terms and definitions, or questions and answers. Let's look at an example of a set of terms and definitions:

```
soliloquy
In drama, where a character speaks to themselves, representing their inner thoughts or feelings and in the process relaying them to the audience (but not to other characters.)
monologue
In drama, where a character speaks their thoughts out loud to share them with the audience and any other characters present.
aside
In drama, where a character shares a comment only with the audience for humorous or dramatic effect. This is usually a feeling, thought or piece of additional background information
```

Description lists use a different wrapper than the other list types — [`<dl>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dl); in addition each term is wrapped in a [`<dt>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dt) (description term) element, and each description is wrapped in a [`<dd>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dd) (description definition) element.

#### [Description list example](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#description_list_example) <a href="#description_list_example" id="description_list_example"></a>

Let's finish marking up our example:

```
<dl>
  <dt>soliloquy</dt>
  <dd>In drama, where a character speaks to themselves, representing their inner thoughts or feelings and in the process relaying them to the audience (but not to other characters.)</dd>
  <dt>monologue</dt>
  <dd>In drama, where a character speaks their thoughts out loud to share them with the audience and any other characters present.</dd>
  <dt>aside</dt>
  <dd>In drama, where a character shares a comment only with the audience for humorous or dramatic effect. This is usually a feeling, thought, or piece of additional background information.</dd>
</dl>
```

Copy to Clipboard

The browser default styles will display description lists with the descriptions indented somewhat from the terms.

#### [Multiple descriptions for one term](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#multiple_descriptions_for_one_term) <a href="#multiple_descriptions_for_one_term" id="multiple_descriptions_for_one_term"></a>

Note that it is permitted to have a single term with multiple descriptions, for example:

```
<dl>
  <dt>aside</dt>
  <dd>In drama, where a character shares a comment only with the audience for humorous or dramatic effect. This is usually a feeling, thought, or piece of additional background information.</dd>
  <dd>In writing, a section of content that is related to the current topic, but doesn't fit directly into the main flow of content so is presented nearby (often in a box off to the side.)</dd>
</dl>
```

Copy to Clipboard

#### [Active learning: Marking up a set of definitions](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#active_learning_marking_up_a_set_of_definitions) <a href="#active_learning_marking_up_a_set_of_definitions" id="active_learning_marking_up_a_set_of_definitions"></a>

It's time to try your hand at description lists; add elements to the raw text in the _Input_ field so that it appears as a description list in the _Output_ field. You could try using your own terms and descriptions if you like.

If you make a mistake, you can always reset it using the _Reset_ button. If you get really stuck, press the _Show solution_ button to see the answer.

### [Quotations](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#quotations) <a href="#quotations" id="quotations"></a>

HTML also has features available for marking up quotations; which element you use depends on whether you are marking up a block or inline quotation.

#### [Blockquotes](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#blockquotes) <a href="#blockquotes" id="blockquotes"></a>

If a section of block level content (be it a paragraph, multiple paragraphs, a list, etc.) is quoted from somewhere else, you should wrap it inside a [`<blockquote>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/blockquote) element to signify this, and include a URL pointing to the source of the quote inside a [`cite`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/blockquote#attr-cite) attribute. For example, the following markup is taken from the MDN `<blockquote>` element page:

```
<p>The <strong>HTML <code>&lt;blockquote&gt;</code> Element</strong> (or <em>HTML Block
Quotation Element</em>) indicates that the enclosed text is an extended quotation.</p>
```

Copy to Clipboard

To turn this into a block quote, we would just do this:

```
<p>Here below is a blockquote...</p>
<blockquote cite="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/blockquote">
  <p>The <strong>HTML <code>&lt;blockquote&gt;</code> Element</strong> (or <em>HTML Block
  Quotation Element</em>) indicates that the enclosed text is an extended quotation.</p>
</blockquote>
```

Copy to Clipboard

Browser default styling will render this as an indented paragraph, as an indicator that it is a quote; the paragraph above the quotation is there to demonstrate that.

#### [Inline quotations](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#inline_quotations) <a href="#inline_quotations" id="inline_quotations"></a>

Inline quotations work in exactly the same way, except that they use the [`<q>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/q) element. For example, the below bit of markup contains a quotation from the MDN `<q>` page:

```
<p>The quote element — <code>&lt;q&gt;</code> — is <q cite="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/q">intended
for short quotations that don't require paragraph breaks.</q></p>
```

Copy to Clipboard

Browser default styling will render this as normal text put in quotes to indicate a quotation, like so:

#### [Citations](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#citations) <a href="#citations" id="citations"></a>

The content of the [`cite`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/blockquote#attr-cite) attribute sounds useful, but unfortunately browsers, screenreaders, etc. don't really do much with it. There is no way to get the browser to display the contents of `cite`, without writing your own solution using JavaScript or CSS. If you want to make the source of the quotation available on the page you need to make it available in the text via a link or some other appropriate way.

There is a [`<cite>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/cite) element, but this is meant to contain the title of the resource being quoted, e.g. the name of the book. There is no reason, however, why you couldn't link the text inside `<cite>` to the quote source in some way:

```
<p>According to the <a href="/en-US/docs/Web/HTML/Element/blockquote">
<cite>MDN blockquote page</cite></a>:
</p>

<blockquote cite="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/blockquote">
  <p>The <strong>HTML <code>&lt;blockquote&gt;</code> Element</strong> (or <em>HTML Block
  Quotation Element</em>) indicates that the enclosed text is an extended quotation.</p>
</blockquote>

<p>The quote element — <code>&lt;q&gt;</code> — is <q cite="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/q">intended
for short quotations that don't require paragraph breaks.</q> -- <a href="/en-US/docs/Web/HTML/Element/q">
<cite>MDN q page</cite></a>.</p>
```

Copy to Clipboard

Citations are styled in italic font by default.

#### [Active learning: Who said that?](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#active_learning_who_said_that) <a href="#active_learning_who_said_that" id="active_learning_who_said_that"></a>

Time for another active learning example! In this example we'd like you to:

1. Turn the middle paragraph into a blockquote, which includes a `cite` attribute.
2. Turn "The Need To Eliminate Negative Self Talk" in the third paragraph into an inline quote, and include a `cite` attribute.
3. Wrap the title of each source in `<cite>` tags and turn each one into a link to that source.

The citation sources you need are:

-   http://www.brainyquote.com/quotes/authors/c/confucius.html for the Confucius quote
-   http://example.com/affirmationsforpositivethinking for "The Need To Eliminate Negative Self Talk".

If you make a mistake, you can always reset it using the _Reset_ button. If you get really stuck, press the _Show solution_ button to see the answer.

### [Abbreviations](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#abbreviations) <a href="#abbreviations" id="abbreviations"></a>

Another fairly common element you'll meet when looking around the Web is [`<abbr>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/abbr) — this is used to wrap around an abbreviation or acronym, and provide a full expansion of the term (included inside a [`title`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes#attr-title) attribute.)

#### [Abbreviation example](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#abbreviation_example) <a href="#abbreviation_example" id="abbreviation_example"></a>

Let's look at an example.

```
<p>We use <abbr title="Hypertext Markup Language">HTML</abbr> to structure our web documents.</p>

<p>I think <abbr title="Reverend">Rev.</abbr> Green did it in the kitchen with the chainsaw.</p>
```

Copy to Clipboard

These will come out looking something like this (the expansion will appear in a tooltip when the term is hovered over):

**Note:** Earlier versions of html also included support for the [`<acronym>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/acronym) element, but it was removed from the HTML spec in favor of using `<abbr>` to represent both abbreviations and acronyms. `<acronym>` should not be used.

#### [Active learning: marking up an abbreviation](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#active_learning_marking_up_an_abbreviation) <a href="#active_learning_marking_up_an_abbreviation" id="active_learning_marking_up_an_abbreviation"></a>

For this simple active learning assignment, we'd like you to mark up an abbreviation. You can use our sample below, or replace it with one of your own.

### [Marking up contact details](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#marking_up_contact_details) <a href="#marking_up_contact_details" id="marking_up_contact_details"></a>

HTML has an element for marking up contact details — [`<address>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/address). This wraps around your contact details, for example:

```
<address>
  Chris Mills, Manchester, The Grim North, UK
</address>
```

Copy to Clipboard

It could also include more complex markup, and other forms of contact information, for example:

```
<address>
  <p>
    Chris Mills<br>
    Manchester<br>
    The Grim North<br>
    UK
  </p>

  <ul>
    <li>Tel: 01234 567 890</li>
    <li>Email: me@grim-north.co.uk</li>
  </ul>
</address>
```

Copy to Clipboard

Note that something like this would also be OK, if the linked page contained the contact information:

```
<address>
  Page written by <a href="../authors/chris-mills/">Chris Mills</a>.
</address>
```

Copy to Clipboard

**Note:** The [`<address>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/address) element should only be used to provide contact information for the document contained with the nearest [`<article>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article) or [`<body>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body) element. It would be correct to use it in the footer of a site to include the contact information of the entire site, on inside an article for the contact details of the author, but not to mark up a list of addresses unrelated to the content of that page.

### [Superscript and subscript](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#superscript_and_subscript) <a href="#superscript_and_subscript" id="superscript_and_subscript"></a>

You will occasionally need to use superscript and subscript when marking up items like dates, chemical formulae, and mathematical equations so they have the correct meaning. The [`<sup>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/sup) and [`<sub>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/sub) elements handle this job. For example:

```
<p>My birthday is on the 25<sup>th</sup> of May 2001.</p>
<p>Caffeine's chemical formula is C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>.</p>
<p>If x<sup>2</sup> is 9, x must equal 3 or -3.</p>
```

Copy to Clipboard

The output of this code looks like so:

### [Representing computer code](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#representing_computer_code) <a href="#representing_computer_code" id="representing_computer_code"></a>

There are a number of elements available for marking up computer code using HTML:

-   [`<code>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/code): For marking up generic pieces of computer code.
-   [`<pre>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/pre): For retaining whitespace (generally code blocks) — if you use indentation or excess whitespace inside your text, browsers will ignore it and you will not see it on your rendered page. If you wrap the text in `<pre></pre>` tags however, your whitespace will be rendered identically to how you see it in your text editor.
-   [`<var>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/var): For specifically marking up variable names.
-   [`<kbd>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/kbd): For marking up keyboard (and other types of) input entered into the computer.
-   [`<samp>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/samp): For marking up the output of a computer program.

Let's look at a few examples. You should try having a play with these (try grabbing a copy of our [other-semantics.html](https://github.com/mdn/learning-area/blob/master/html/introduction-to-html/advanced-text-formatting/other-semantics.html) sample file):

```
<pre><code>var para = document.querySelector('p');

para.onclick = function() {
  alert('Owww, stop poking me!');
}</code></pre>

<p>You shouldn't use presentational elements like <code>&lt;font&gt;</code> and <code>&lt;center&gt;</code>.</p>

<p>In the above JavaScript example, <var>para</var> represents a paragraph element.</p>

<p>Select all the text with <kbd>Ctrl</kbd>/<kbd>Cmd</kbd> + <kbd>A</kbd>.</p>

<pre>$ <kbd>ping mozilla.org</kbd>
<samp>PING mozilla.org (63.245.215.20): 56 data bytes
64 bytes from 63.245.215.20: icmp_seq=0 ttl=40 time=158.233 ms</samp></pre>
```

Copy to Clipboard

The above code will look like so:

### [Marking up times and dates](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting#marking_up_times_and_dates) <a href="#marking_up_times_and_dates" id="marking_up_times_and_dates"></a>

HTML also provides the [`<time>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/time) element for marking up times and dates in a machine-readable format. For example:

```
<time datetime="2016-01-20">20 January 2016</time>
```

{% embed url="https://gist.github.com/bgoonz/9baea4821996ec8449a04133003b1ae0" %}
