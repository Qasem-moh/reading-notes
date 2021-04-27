
![link](https://1.bp.blogspot.com/-TZqlIKhGRaQ/VubNV0HuMzI/AAAAAAAAG6c/d7DWNFoX3w87luF3-ye_hE23R7PNRMDgg/s100/link.png)
# **Links**

_A link (short for hyperlink) is an HTML object that allows you to jump to a new location when you click or tap it. Links are found on almost every webpage and provide a simple means of navigating between pages on the web._

_Links can be attached to text, images, or other HTML lements. Most text links are blue since that is the standard color web browsers use to display links. However, links can be any color since the style of the link text may be_ _customized using HTML or CSS styles. In the early days of the web, links were underlined by default. Today, underlining links is less common._

_When a link is applied to an image, the link tag encapsulates or surrounds the image tag. Since the image tag is nested inside the link tag, the image itself becomes a link. This method can be used to apply links to other elements such as <div'> and <span'> objects. However, since CSS can be used to stylize a link, an <a'> tag with a CSS class or ID attribute is often used in place of a <div> or <span> tag._


_Below is an example of the HTML for a text and image link:_

Text Link: <a href="/definition/computer">Computer Definition</a>

Image Link: <a href="https://techterms.com/definition/computer"><img src="/images/computer.jpg" alt="desktop PC"></a>

## Relative and Absolute Links

![Relative and Absolute Links](https://www.rankmovers.com/wp-content/uploads/2020/08/Absolute-vs-relative-example-to-use.jpg)

_The first link above is a "relative link" because it does not include the domain name. Instead the link is relative to the current website. Any internal link on TechTerms.com, for example, does not need "https://techterms.com/" in the source. Rather, a relative link like "/definition/computer" is all that is required. Since the link starts with a forward slash, the path begins with the root directory. If a relative link does not start with a forward slash, the path is relative to the current URL._

_The second link above is an absolute link because it includes the domain name. Absolute links are required for external links, which direct you to another website. They may begin with "http" or "https." Absolute links may also begin with two forward slashes ("//"). This is interpreted as "http://" for pages served via HTTP and "https://" for pages served via HTTPS._

_NOTE: The "a" in the <a'> tag stands for "anchor," since early hypertext documents often linked to anchors (or markers) within a page rather than other pages. The "href" within an <a'> stands for "hypertext reference."_
***
_A webpage can contain various links that take you directly to other pages and even specific parts of a given page. These links are known as hyperlinks._

_Hyperlinks allow visitors to navigate between Web sites by clicking on words, phrases, and images. Thus you can create hyperlinks using text or images available on a webpage._

_Note − I recommend you to go through a short tutorial on Understanding URL_

**Linking Documents** 

_A link is specified using HTML tag <a'>. This tag is called anchor tag and anything between the opening <a'> tag and the closing </a'> tag becomes part of the link and a user can click that part to reach to the linked document. Following is the simple syntax to use <a'> tag._

![](https://lorelle.files.wordpress.com/2015/03/links-html-anchor-tag-code-breakdown-lorelle-wordpress-school.png?w=1024&h=509)

## HTML - Email Links


_It is not difficult to put an HTML email link on your webpage but it can cause unnecessary spamming problem for your email account. There are people, who can run programs to harvest these types of emails and later use them for spamming in various ways._

_You can have another option to facilitate people to send you emails. One option could be to use HTML forms to collect user data and then use PHP or CGI script to send an email._

_A simple example, check our Contact Us Form. We take user feedback using this form and then we are using one CGI program which is collecting this information and sending us email to the one given email ID._

_Note − You will learn about HTML Forms in HTML Forms and you will learn about CGI in our another tutorial Perl CGI Programming._

## HTML Email Tag
_HTML <a'> tag provides you option to specify an email address to send an email. While using <a'> tag as an email tag, you will use mailto: email address along with href attribute. Following is the syntax of using mailto instead of using http._
<a href = "mailto:qasemcoder2020@gmailcom">Send Email</a>
![email](https://i.ibb.co/s119bRm/Screenshot-from-2021-04-27-18-46-16.png)


![](https://i.stack.imgur.com/5Pg9B.png)
***
## position

_CSS helps you to position your HTML element. You can put any HTML element at whatever location you like. You can specify whether you want the element positioned relative to its natural position in the page or absolute based on its parent element._

_Now, we will see all the CSS positioning related properties with examples −_

_Relative Positioning_
_Relative positioning changes the position of the HTML element relative to where it normally appears. So "left:20" adds 20 pixels to the element's LEFT position._

_You can use two values top and left along with the position property to move an HTML element anywhere in the HTML document._

* Move Left - Use a negative value for left.
* Move Right - Use a positive value for left.
* Move Up - Use a negative value for top.
* Move Down - Use a positive value for top.

**Values**

_**static**: every element has a static position by default, so the element will stick to the normal page flow. So if there is a left/right/top/bottom/z-index set then there will be no effect on that element._

_**relative**: an element’s original position remains in the flow of the document, just like the static value. But now left/right/top/bottom/z-index will work. The positional properties “nudge” the element from the original position in that direction._

_**absolute**: the element is removed from the flow of the document and other elements will behave as if it’s not even there whilst all the other positional properties will work on it._

_**fixed**: the element is removed from the flow of the document like absolutely positioned elements. In fact they behave almost the same, only fixed positioned elements are always relative to the document, not any particular parent, and are unaffected by scrolling._

_**sticky** (experimental): the element is treated like a relative value until the scroll location of the viewport reaches a specified threshold, at which point the element takes a fixed position where it is told to stick._

_**inherit**: the position value doesn’t cascade, so this can be used to specifically force it to, and inherit the positioning value from its parent._

![](https://hackernoon.com/drafts/t2w3yae.png)


## Functions

_Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it._

**Function declarations**

![](https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/declaration.svg)

_A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:_

_The name of the function._
_A list of parameters to the function, enclosed in parentheses and separated by commas._
_The JavaScript statements that define the function, enclosed in curly brackets, {...}._
_For example, the following code defines a simple function named square:_


function square(number) {
  return number * number;
}

_The function square takes one parameter, called number. The function consists of one statement that says to return the parameter of the function (that is, number) multiplied by itself. The statement return specifies the value returned by the function:_

_return number * number;_

_The function square takes one parameter, called number. The function consists of one statement that says to return the parameter of the function (that is, number) multiplied by itself. The statement return specifies the value returned by the function:_

**return number * number;**


_Primitive parameters (such as a number) are passed to functions by value; the value is passed to the function, but if the function changes the value of the parameter, this change is not reflected globally or in the calling function._

_If you pass an object (i.e. a non-primitive value, such as Array or a user-defined object) as a parameter and the function changes the object's properties, that change is visible outside the function, as shown in the following example:_
![](https://i.ytimg.com/vi/bkKuqKASG_8/maxresdefault.jpg)


