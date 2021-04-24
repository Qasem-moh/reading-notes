# How People Access the Web
_People access websites using software called a web browser. Popular examples include Firefox, Internet Explorer, Safari, Chrome, and Opera._
![](https://mqalaat.net/images/8/8b/%D8%A7%D9%81%D8%B6%D9%84_%D9%85%D8%AA%D8%B5%D9%81%D8%AD%D8%A7%D8%AA_%D9%84%D9%84%D9%83%D9%85%D8%A8%D9%8A%D9%88%D8%AA%D8%B1.jpg)
<br/>

_In order to view a web page, users might type a web address
into their browser, follow a link from another site, or use a
bookmark._

# Web Servers
When you ask your browser for a web page, the request is sent across the Internet to a special computer known as a web server which hosts the website

_The term web server can refer to hardware or software, or both of them working together._

1. On the hardware side, a web server is a computer that stores web server software and a website's component files. (for example, HTML documents, images, CSS stylesheets, and JavaScript files) A web server connects to the Internet 
and supports physical data interchange with other devices connected to the web.

2. On the software side, a web server includes several parts that control how web users access hosted files. At a minimum, this is an HTTP server. An HTTP server is software that understands URLs (web addresses) and HTTP (the protocol your browser uses to view webpages). An HTTP server can be accessed through the domain names of the websites it stores, and it delivers the content of these hosted websites to the end user's device.

_At the most basic level, whenever a browser needs a file that is hosted on a web server, the browser requests the file via HTTP. When the request reaches the correct (hardware) web server, the (software) HTTP server accepts the request, finds the requested document, and sends it back to the browser, also through HTTP. (If the server doesn't find the requested document, it returns a 404 response instead.)_

![](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_web_server/web-server.svg)

***
To publish a website, you need either a static or a dynamic web server.

A static web server, or stack, consists of a computer (hardware) with an HTTP server (software). We call it "static" because the server sends its hosted files as-is to your browser.

A dynamic web server consists of a static web server plus extra software, most commonly an application server and a database. We call it "dynamic" because the application server updates the hosted files before sending content to your browser via the HTTP server.

For example, to produce the final webpages you see in the browser, the application server might fill an HTML template with content from a database. Sites like MDN or Wikipedia have thousands of webpages. Typically, these kinds of sites are composed of only a few HTML templates and a giant database, rather than thousands of static HTML documents. This setup makes it easier to maintain and deliver the content.
 ***


 _Webpages can and will look pretty different from one another, but they all tend to share similar standard components, unless the page is displaying a fullscreen video or game, is part of some kind of art project, or is just badly structured:_

**header:**

_Usually a big strip across the top with a big heading, logo, and perhaps a tagline. This usually stays the same from one webpage to another.
navigation bar:_

**Links** to the site's main sections; usually represented by menu buttons, links, or tabs. Like the header, this content usually remains consistent from one webpage to another — having inconsistent navigation on your website will just lead to confused, frustrated users. Many web designers consider the navigation bar to be part of the header rather than an individual component, but that's not a requirement; in fact, some also argue that having the two separate is better for accessibility, as screen readers can read the two features better if they are separate.

**main content:**
A big area in the center that contains most of the unique content of a given webpage, for example, the video you want to watch, or the main story you're reading, or the map you want to view, or the news headlines, etc. This is the one part of the website that definitely will vary from page to page!

**sidebar:**
Some peripheral info, links, quotes, ads, etc. Usually, this is contextual to what is contained in the main content (for example on a news article page, the sidebar might contain the author's bio, or links to related articles) but there are also cases where you'll find some recurring elements like a secondary navigation system.

**footer:**
A strip across the bottom of the page that generally contains fine print, copyright notices, or contact info. It's a place to put common information (like the header) but usually, that information is not critical or secondary to the website itself. The footer is also sometimes used for **SEO** purposes, by providing links for quick access to popular content.
A "typical website" could be structured something like this:
![](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure/sample-website.png)

***
**DOCTYPEs** 

_Source text Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using (although browsers usually display the page even if it is not included). We will therefore be including one in each example for the rest of the bo As you will see when we come to look at CSS and its box model on
page 316, the use of a DOCTYPE can also help the browser to render a page correctly.Because XHTML was written in XML, you will sometimes see pages that use the XHTML strict DOCTYPE start with the optional XML declaration.
Where this is used, it should be the first thing in a document. There must be nothing before it, not even a space. _
 
![](https://i.ibb.co/4fz89Lq/erty.png)
***
**Comments Article**
<!-- -->
_If you want to add a comment to your code that will not be
visible in the user's browser, you can add the text between these
characters:_
<!-- comment goes here -->
_It is a good idea to add comments to your code because,no matter how familiar you are with the page at the time of writing it, when you come back to it later (or if someone else needs to look at the code), comments will make it much easier to understand. Although comments are not visible to users in the main browser window, they can be viewed by anyone who looks at the source code behind the page. On a long page you will often see comments used to indicate
where sections of the page start or end, and to pass on notes to help anyone who is looking at the code understand it. Comments can also be used
around blocks of code to stop that code from being displayed in the browser. In the example on the left, the email link has been commented out._
![Comments](https://i.ibb.co/dP2sNNt/image.png)
***
**ID Attribute**

_Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore (not a number or any other character).
It is important that no two elements on the same page have the same value for their id attributes (otherwise the value is no longer unique)._

![ID](https://i.ibb.co/1zLqX3w/1.png)

***
**Class Attribute**
_Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements as being different from the other elements on the page. For example, you might have some paragraphs of text that contain information that is more important than others and want to distinguish these elements, or you might want to differentiate between links that point to other
pages on your own site and links that point to external sites. To do this you can use the class attribute. Its value should describe the class it belongs to. In the example on the left, key paragraphs have a class attribute whose value is important . The class attribute on any element can share the same
value. So, in this example, the value of important could be used on headings and links, too._
![Class](https://i.ibb.co/Ntyfb47/2.png)
***
**Traditional HTML Layouts** 

For a long time, web page authors used <div> elements to group together related elements on the page (such as the elements that form a **header**, an article, footer or sidebar). Authors used class or id attributes to indicate the role of the //<div>// element in the structure of the page. 
***
On the right you can see a layout that is quite common (particularly on blog sites). At the top of the page is the header, containing a logo and the
primary navigation. Under this are one or more articles or posts. Sometimes
these are summaries that link to individual posts. There is a side bar on the right- hand side (perhaps featuring a search option, links to other recent articles, other sections of the site, or even ads). When coding a site like this, developers would usually put these main sections of the page inside <div> elements and use the class or id attributes to indicate the purpose of that part of the page.
![](https://i.ibb.co/dGHLt1F/3.png)
***
**New Html5 Layout Elements**

_HTML5 introduces a new set of elements that allow you to divide up the
parts of a page. The names of these elements indicate the kind of content
you will find in them. They are still subject to change, but that has not
stopped many web page authors using them already._

_This example has exactly the same structure as seen on the previous page. However, many of the <div> elements have been replaced by new HTML5 layout
elements._

_For example, the header sits inside a new <header> element,the navigation in a <nav> element, and the articles are in individual <article> elements._

_The point of creating these new elements is so that web page authors can use them to help describe the structure of the page. For example, screen reader software might allow users to ignore headers and footers and get straight to
the content. Similarly, search engines might place more weight on the content in an <article> element than that in the <header> or <footer> elements. I think you will agree that it also makes the code easier to follow._

![Html5](https://i.ibb.co/ZM5qhCn/4.png)
***

