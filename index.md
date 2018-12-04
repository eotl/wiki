---
wikiWrapper: IndexArticle
wikiComponents: 
  - TableOfContents
title: EotL Wiki
description: EotL wiki overview.
see:
  - MUDs
  - Getting Started
---

It's a dangerous world out there, but this wiki should supply you all the critical information you need to survive your adventure on EotL. To contribute, you can mudmail Devo with your content suggestions, or go right to the source by requesting access to the [Github repository](https://github.com/eotl/wiki). 

{{ <TableOfContents {...props} depth={2} /> }}

Articles are organized into a folder structure which is reflected as "categories" while browsing the wiki. If you browse to or search for a category page, the index.md file in that folder will be displayed. Categories without an index article will show a blank page using the IndexArticle wrapper, which includes sections for member articles and subcategories, such as the page you're viewing right now.

The remainder of this document will describe how to write the articles themselves.

### Markdown
The wiki is written in Markdown with additional support for harnessing content from EotL's web component library. If you need help getting started with Markdown syntax, check out this [cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). The rest of this document will assume you're familiar with the basics. The source code for this document can be viewed on [Github](https://raw.githubusercontent.com/eotl/wiki/master/index.md).

### Links
There are a few different ways to specify links in your article content. For external links such as the ones displayed above, the standard Markdown link syntax is sufficient. 

For internal links, you will want to use the &lt;Link/&gt; tag instead of the standard Markdown links to render the new content internally instead of performing a full page refresh. This method uses the special JSX interpolation syntax with the tag enclosed in double braces, such as {{ <Link to="/">this home page link</Link> }}. By default, the &lt;Link/&gt; component will be imported on all wiki pages.

You can also link directly to other wiki articles by using the double bracket syntax, such as this link to [[Eternal City]], or this other one with [[Eternal City:alternate link text]]. The target inside the double brackets will be matched against the article's _filename_, not its title, with the value lowercased and its spaces converted to underscores.

### Front Matter
Front matter is a special data section at the top of your wiki article specified in [YAML syntax](http://yaml.org/start.html) which you can include to specify how you want your page to be rendered.

#### title
The title value specifies the page title to be displayed in headers and in navigational elements like links and buttons. If you don't set a title, one will be calculated based on the article's file name.

#### description
The description value is a short phrase or sentence which describes the article content, and often appears with the title as a caption or subtitle. If no description is provided, the default behavior is to display nothing where a description would normally appear. However, based on the page type, a default description may be generated. For instance, category indexes will get a default description which consists of their subcategories and articles.

#### see
The see value lists which articles to link to in this article's "See also" section. The list values will be matched against an article's _filename_, not its title, with the value lowercased and spaces its spaces converted to underscores.

#### wikiWrapper
The wikiWrapper value is a JavaScript component which will enclose your page content. Depending on which wrapper you specify, your page may automatically get special content like navigational elements or dynamically generated subsections. If you don't specify a wrapper, your document will be displayed as-is.

Different wrapper components can be used for different types of articles to automatically generate surrounding content, such as headers, footers, and sidebars. While you can entirely forgo specifying a wrapper and format the entire article yourself, it's recommended to share wrappers across articles that have the same format for the sake of uniformity and ease of maintenance. 

##### BasicArticle
The basic article wrapper contains the standard header and a "See also" section for any articles specified in the 'see' front matter. It also supplies breadcrumbs and a sidebar for browsing the article tree.

##### IndexArticle
Used for category indexes, index articles are like basic articles but also contain sections for subcategory and member article lists.

##### TextArticle
Text articles are written in plain text and displayed in monospace. Most of these articles were ported over from the MUD and need to be re-written in Markdown.

##### StubArticle
Article stubs are placeholders for future articles. If you're looking to contribute, expanding the stubs is a good place to start.

#### wikiComponents
In addition to wrapper components, you may import other smaller components you can embed in the body of your article. If you find yourself using the same patterns over and over again across different wiki pages, it may be useful to converting them to components.

##### TableOfContents
The table of contents component will scan the headings in your document and generate a table of contents which has jump links to the different sections. The table of contents component takes an optional parameter 'depth' to specify how many levels deep your want your table of contents to be.

#### muiComponents
The EotL website uses the Material UI framework to lay out components, configure typeset, and build user interactions. While the entire framework is quite extensive, there are a few common components you may find useful in your pages.

##### Paper
The Paper component displays your content on an elevated sheet of "paper" to make it stand out against the surrounding content. The table of contents component on this page and the footer links below are examples of it in use. See the [Material UI website](https://material-ui.com/demos/paper/) for a longer explanation.

##### Grid
The Grid component allows you to lay out components side-by-side, in a grid configuration. Each item should be surrounded by &lt;Grid item&gt;&lt;/Grid&gt; tags, and the entire grid should be surrounded by a &lt;Grid container&gt;&lt;/Grid&gt; tag. See the [Material UI website](https://material-ui.com/layout/grid/) for a longer explanation.

#### muiIcons
The muiIcons value lets you import Material UI icons for display on your page. You can view the available icon set on [their website](https://material.io/tools/icons/).
