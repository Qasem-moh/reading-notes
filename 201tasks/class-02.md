# Basics of HTML, CSS & JS

_When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.
TEXT
● ● Structural markup: the elements that you can use to
describe both headings and paragraphs
● ● Semantic markup: which provides extra information; such
as where the emphasis is placed in a sentence, that something
you have written is a quotation (and who said it), the
meaning of acronyms, and so on_

---

**Headings**

_HTML headings are part of the HTML used to display your website, the code behind the content. The code of your page can contain headings and other tags, which are used to identify and style the content.
The heading tags range from H1 to H6. With H1 being the most important heading on the page. The majority of content on your pages should be in <p> tags for paragraph, and these can follow each heading tag._

![Heading](https://www.schudio.com/wp-content/uploads/2016/10/html-headings.png?x43850)

## HTML Headings - Why are they useful?

HTML headings achieve two main things when used on websites, and both are about making your website better and easier to understand and read.

* **Changing appearance with HTML Headings**

    _The first is benefit is changing the appearance of the text within the tag. Using a HTML heading tag makes the text look like a header, especially when using a lower numbered header tag e.g. H1 and H2. Visitors to your website can easily tell the difference between header and body content and what level of header it is - text in a H3 heading tag will be smaller than text in a H2 heading tag. It also helps to keep your site looking consistent and future proof._


* **Consistent**
    _Maintaining a consistent appearance and clear structure is easier with HTML headings because their styling for your site is set centrally and then applied to all instances of the heading tags. Using the same style of headings and making sure your content is broken up will hugely improve the readability and usability of your website._

* **Future proof**

    _Because the HTML headings pull their appearance and styling from the central location where the styles are defined for your site, when your website gets updated any content styled with header tags will automatically be updated to match the new look._

* **SEO (Search Engine Optimisation)** 

    _The second benefit is your search engine ranking. Tagging and identifying your content makes your pages easier for search engines read, and apply priorities to the different content on your site. Google (other search engines are available) is trying to provide you the answer to a search term as best as it can._
    _"Larry Page, Google's co-founder, once described the “perfect search engine” as something that “understands exactly what you mean and gives you back exactly what you want.”"**_
    _Applying your HTML heading tags correctly helps google and other search engines to identify which bits of your content titles, and in broad strokes what your content is about. The better it knows this the higher your page will appear in search results for relevant queries._

***
**Paragraphs**

![Paragraphs](https://www.tahirtaous.com/wp-content/uploads/2015/03/HTMl-for-Beginner-2.png)
_The Paragraph element_
_The HTML <> element represents a paragraph. Paragraphs are usually represented in visual media as blocks of text separated from adjacent blocks by blank lines and/or first-line indentation, but HTML paragraphs can be any structural grouping of related content, such as images or form fields._

_Paragraphs are block-level elements, and notably will automatically close if another block-level element is parsed before the closing </> tag. See “Tag omission” below._
***

**Bold & Italic**
_Two more tags that come in useful are the Bold and Italic tags. They are quite easy to use. Here are the Bold tags:_
<B'> </B'>

_And here are the Italic tags:_

<i'> </i'>

_The text you want to change goes between the two tags:_

<B'> ... Rest of Hamlet's Soliloquy goes here</B>

<i'> ... Rest of Hamlet's Soliloquy goes here</i>

If you want Bold and Italic text then you can nest the two:

<B'><i'> ... Rest of Hamlet's Soliloquy goes here</i></B>

_The two I tags go between the two B tags. You can have it the other way around, though, with the I tags first:_

<i'><B'> ... Rest of Hamlet's Soliloquy goes here</B></i>

_Be careful of this, however:_

<i'><B'> ... Rest of Hamlet's Soliloquy goes here</i></B>

_This is a mismatched pair of tags. The two tags on the inside are B and I, and the ones on the outside are I and B. A modern browser will probably correct the mismatch, but older ones may not._
***
**Superscript Article & Subscript**
_Subscript: The <sub'> tag is used to add a subscript text to the HTML document. The <sub'> tag defines the subscript text. Subscript text appears half a character below the normal line and is sometimes rendered in a smaller font. Subscript text can be used for chemical formulas, like H2O to be written as H2O._
_Superscript: The <sup'> tag is used to add a superscript text to the HTML document. The <sup'> tag defines the superscript text. Superscript text appears half a character above the normal line and is sometimes rendered in a smaller font. Superscript text can be used for footnotes._

![sub](https://i.ibb.co/Vx642Tg/1212.png)
**The Result
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-07-at-1.47.12-PM.png)

**Line Breaks Article & Horizontal Rules**

_The <hr'> tag in HTML stands for horizontal rule and is used to insert a horizontal rule or a thematic break in an HTML page to divide or separate document sections. The <hr'> tag is an empty tag and it does not require an end tag._
_Tag Attributes: The table given below describe the <hr'> tag attributes:_

***
**Strong & Emphasis**
_The <strong'> and <em'> tags are used for emphasizing parts of a text. The <strong'> tag should be used to indicate strong importance, seriousness, or urgency, like to indicate key phrases in a text for someone skimming it. The <em'> tag should be used to represent stress emphasis, like when you'd read the emphasized text in a different tone of voice. Both tags can be used together, where it makes sense._

![Strong](https://i.ytimg.com/vi/ymZFOCfxkvg/maxresdefault.jpg)
![Emphasis](https://www.wikitechy.com/step-by-step-html-tutorials/img/html-images/code-explanation-em-tag-in-html.png)
***
## Understanding CSS:

_The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element._
_On this page, you can see a basic HTML page. On the right hand page, you can see the same HTML page, but I have added outlines to each of the elements so that you can see how CSS will treat each element as if it lives inside its own box._


**CSS Associates Style rules with HTML elements**

_CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rulecontains two parts: a selector and a declaration._
![](https://images.slideplayer.com/32/9811421/slides/slide_5.jpg).

**CSS Properties Affect How Elements Are Displayed**
_CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon._ 

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTYQKrKOgeeAEFQVGhH1dG5H1wIFz_CnVyQP1UKj6H90rK5-GwPStt-W-KnvrgpetXuaqQ&usqp=CAU)