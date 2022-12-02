***<h1 align="center">HTML (Hypertext Markup Language)</h1>***
# ***Important Links***
***[Special](https://html.spec.whatwg.org/multipage/indices.html#element-content-categories)***
## ***Q1. The History of HTML***
*HTML was first created by Tim Berners-Lee, Robert Cailliau, and others starting in `1989`. It stands for Hyper Text Markup Language.*

*`HTML is a Hypertext markup language` that defines the structure of your content. HTML consists of a series of elements, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way. The enclosing tags can make a word or image hyperlink to somewhere else, can italicize words, can make the font bigger or smaller, and so on.*
* *Hypertext:- "Hypertext" refers to links that connect web pages to one another, either within a single website or between websites. Links are a fundamental aspect of the Web. By uploading content to the Internet and linking it to pages created by other people, you become an active participant in the World Wide Web.*
* *Markup :- HTML uses "markup" to annotate text, images, and other content for display in a Web browser. HTML markup includes special "elements" such as  <title>, </title> and many others.*
* ***HTML Versions***
    * *`HTML 1.0`: The first version of HTML was 1.0, which was the barebones version of HTML language, and it was released in1991.*
    * *`HTML 2.0`: This was the next version which was released in 1995, and it was standard language version for website design. HTML 2.0 was able to support extra features such as form-based file upload, form elements such as text box, option button, etc.*
    * *`HTML 3.2`: HTML 3.2 version was published by W3C in early 1997. This version was capable of creating tables and providing support for extra options for form elements. It can also support a web page with complex mathematical equations. It became an official standard for any browser till January 1997. Today it is practically supported by most of the browsers.*
    * *`HTML 4.01`: HTML 4.01 version was released on December 1999, and it is a very stable version of HTML language. This version is the current official standard, and it provides added support for stylesheets (CSS) and scripting ability for various multimedia elements.*
    * *`HTML5` : HTML5 is the newest version of HyperText Markup language. The first draft of this version was announced in January 2008. There are two major organizations one is W3C (World Wide Web Consortium), and another one is WHATWG( Web Hypertext Application Technology Working Group) which are involved in the development of HTML 5 version, and still, it is under development.*
* *create html file:- Save the HTML file with .htm or .html extension.*
## ***Q2. What is the <!DOCTYPE>?***
*It defines the document type or it instruct the browser about the version of HTML.*
## ***Q3. What is the &lt;html&gt;?***
*It's a root element of an HTML page. This tag informs the browser that it is an HTML document. Text between html tag describes the web document. It is a container for all other elements of HTML except <!DOCTYPE>.*

## ***Q4. What is the HTML &lt;head&gt;?***
*`The <head> element contains meta information about the HTML page.`*

*This is where all the metadata for the page goes — stuff mostly meant for search engines and other computer programs.*

*The HTML head is the contents of the `<head>` element. Unlike the contents of the `<body>` element (which are displayed on the page when loaded in a browser), the head's content is not displayed on the page. Instead, the head's job is to contain metadata about the document*

*The `<head>` includes the following elements:*
* *The `<title>` tag defines the title of a web page (required). It may be confused with the `<h1>` tag, but they are different. The `<h1> `tag specifies the title of page content, whereas the `<title>` tag is metadata representing the title of the entire HTML content and not its content.*
* *The style tag contains CSS code that defines how HTML elements should be rendered in a browser.*
* *The `<base>` tag defines an absolute (base) URL for all relative URLs.*
* *The `<link>` tag defines the relationship between the current HTML document and the resource to which it refers, or contains a link to an external style sheet. It can have two attributes: rel="stylesheet" and href*
* *The `<meta>` tag provides additional information (metadata) about HTML document. The <head> of a page can include different kinds of `<meta>` elements that may contain name and content attributes*
* *The `<script>` tag contains a script (generally JavaScript), or reference to an external file with scripts.This element may not be included in `<head>`. Sometimes, it is better to put it at the bottom of `<body>`. The `<script>` element may seem empty, but it's not.*
* *The `<noscript>` tag defines an alternate text, which is displayed, if the browser doesn’t support scripts or scripts are disabled by the user.*

## ***Q5. What is the &lt;meta&gt;?***
*This is where information about the document is stored: character encoding, name (page context), description.*

*The `<meta>` element holds information about your page that you want other computers to understand. The contents of this element will not be printed on the page, and are not known to the human reader. They are designed to aid with categorization, search engine indexing and browser behavior.*

## ***Q6. What is the &lt;title&gt;?***
*As its name suggested, it is used to add title of that HTML page which appears at the top of the browser window. It must be placed inside the head tag and should close immediately. (Optional)*
## ***Q7. What is the &lt;body&gt;?***
*The `<body>` element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.*

*Text between body tag describes the body content of the page that is visible to the end user. This tag contains the main content of the HTML document.*

## ***Q8. What is the Tags?***
*An HTML tag surrounds the content and apply meaning to it. It is written between < and > brackets.*
## ***Q9. What is the Attribute?***
*An attribute in HTML provides extra information about the element, and it is applied within the start tag. An HTML attribute contains two fields: name `&` value.*![Alt text](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started/grumpy-cat-attribute-small.png)
## ***Q10. What is the Elements?***
*An HTML element is an individual component of an HTML file. In an HTML file, everything written within tags are termed as HTML elements.*
![element example](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started/grumpy-cat-small.png)

# ***Important***
*Note: Tags in HTML are not case-sensitive. This means they can be written in uppercase or lowercase. For example, a `<title>` tag could be written as `<title>`, `<TITLE>`, `<Title>`, `<TiTlE>`, etc., and it will work. However, it is best practice to write all tags in lowercase for consistency and readability.*

## ***Q11. Block versus inline elements.***
*There are two important categories of elements to know in HTML: block-level elements and inline elements.*
* *Block-level elements form a visible block on a page. A block-level element appears on a new line following the content that precedes it. Any content that follows a block-level element also appears on a new line. Block-level elements are usually structural elements on the page. For example, a block-level element might represent headings, paragraphs, lists, navigation menus, or footers. A block-level element wouldn't be nested inside an inline element, but it might be nested inside another block-level element.*
* Inline elements are contained within block-level elements, and surround only small parts of the document's content (not entire paragraphs or groupings of content). An inline element will not cause a new line to appear in the document. It is typically used with text, for example an `<a>` element creates a hyperlink, and elements such as `<em>` or `<strong>` create emphasis.*

## ***Q12. Void elements?***
*Not all elements follow the pattern of an opening tag, content, and a closing tag. Some elements consist of a single tag, which is typically used to insert/embed something in the document. Such elements are called void elements. For example, the `<img>` element embeds an image file onto a page:*

# ***Important***
*Note: In HTML, there is no requirement to add a / at the end of a void element's tag, for example: `<img src="images/cat.jpg" alt="cat" />`. However, it is also a valid syntax, and you may do this when you want your HTML to be valid XML.*

##  ***Q13. Boolean attributes?***
*Sometimes you will see attributes written without values. This is entirely acceptable. These are called Boolean attributes. Boolean attributes can only have one value, which is generally the same as the attribute name. For example, consider the disabled attribute, which you can assign to form input elements. (You use this to disable the form input elements so the user can't make entries. The disabled elements typically have a grayed-out appearance.)*