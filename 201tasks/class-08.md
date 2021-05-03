# Building Blocks

_HTML (Hypertext Markup Language) elements historically were categorized as either "block-level" elements or "inline-level" elements. Since this is a presentational characteristic it is nowadays specified by CSS in the Flow Layout. A Block-level element occupies the entire horizontal space of its parent element (container), and vertical space equal to the height of its contents, thereby creating a "block". In this article, we'll examine HTML block-level elements and how they differ from inline-level elements.Browsers typically display the block-level element with a new line both before and after the element. You can visualize them as a stack of boxes._

![Blocks](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQb1NALg7H8cu9tBzhPdU0JT1HYzR15h2ELr7M7OcOadJVQQxcg9iSFXuKP-aGSmUGK-tQ&usqp=CAU)

_CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box._

_Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors._
![Blocks](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSJyKrvBdeXSWlVbTI2hBgtmPooSgkKRgL2-jBPdSLlyjw_wa0ZZWb1dJ5gXpYlQUGWdc0&usqp=CAU)
***


## Block-level vs. inline
There are a couple of key differences between block-level elements and inline elements:

**Content model**
_Generally, block-level elements may contain inline elements and (sometimes) other block-level elements. Inherent in this structural distinction is the idea that block elements create "larger" structures than inline elements._

**Default formatting**

_By default, block-level elements begin on new lines, but inline elements can start anywhere in a line._
_The distinction of block-level vs. inline elements was used in HTML specifications up to 4.01. In HTML5, this binary distinction is replaced with a more complex set of content categories. While the "inline" category roughly corresponds to the category of phrasing content, the "block-level" category doesn't directly correspond to any HTML5 content category, but "block-level" and "inline" elements combined together correspond to the flow content in HTML5. There are also additional categories, e.g. interactive content._

***
## Containing Elements

_If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element._

_It is common to group a number of elements together inside a <div'>_
_(or other block-level) element. For example, you might group_ _together  all of the elements that form the header of a site (such as the logo and the main navigation). The <div'> element that contains this group of elements is then referred to as the containing element_

## Controlling the Position of Elements

CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property

* **Normal flow**
Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-by-side, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else).

* **Relative Positioning**
This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position, they would be in normal flow.
* **Absolute positioning**
This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position
of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.
* **Fixed Positioning**
This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of
surrounding elements and they do not move when the user scrolls up or down the page.
* **Floating Elements**
Floating an element allows you to take that element out of the normal flow and position it to the far left or right of a containing box. They floated element becomes a block-level element around which other content can flow