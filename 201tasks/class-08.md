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
1- **position:static**
In normal flow, each block-level element sits on top of the next
one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate
those elements should appear in normal flow, but the syntax
would be:
**position: static;**
I have not specified a width property for the heading element, so you can see how it stretches the width of the entire browser window by default. The paragraphs are restricted to 450 pixels wide. This shows
how the elements in normal flow start on a new line even if they
do not take up the full width of the browser window

* **Relative Positioning**
This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position, they would be in normal flow.
1- **position:relative**
Relative positioning moves an element in relation to where it would have been in normal flow. For example, you can move it 10 pixels lower than it would have been in normal flow or 20% to
the right. You can indicate that an element should be relatively positioned using the position property with a value of relative. You then use the offset properties ( top or bottom and left or right ) to indicate how far to move the element from where it would have been in normal flow. To move the box up or down, you can use either the top or bottom properties. To move the box horizontally, you can use either the left or right properties. The values of the box offset properties are usually given in pixels, percentages, or ems.
* **Absolute positioning**
This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position
of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.
1- **position:absolute**
When the position property is given a value of absolute, the box is taken out of the normal flow and no longer affects the position of other elements on the page. (They act like it is not there.) The box offset properties ( top or bottom and left or right ) specify where the element should appear in relation to its containing element. In this example, the heading has been positioned at the top of the page and 500 pixels from its left edge. The width of the heading is set to be 250 pixels wide. The width property has also been applied to the <'p'> elements in this example to prevent the text from overlapping and becoming unreadable. By default, most browsers add a margin to the top of the <'h1'> element. This is why there is a gap between the top of the browser and the box containing the <'h1'> element. If you wanted to remove this margin, you could add the following code to the
<'h1'> element's style rules: margin: 0px;
* **Fixed Positioning**
This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of
surrounding elements and they do not move when the user scrolls up or down the page.
1- **position:fixed**
Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed . It positions the element in
relation to the browser window. Therefore, when a user scrolls down the page, it stays in the exact same place. It is a good idea to try this example in your browser to see the effect. To control where the fixed position box appears in relation to the browser window, the box
offset properties are used. In this example, the heading has been positioned to the top left-hand corner of the browser window. When the user scrolls down the page, the paragraphs disappear behind the heading. The <p'> elements are in normal flow and ignore the space that the <h1'> element would have taken up. Therefore, the margin-top property has been used to push the first <p'> element below where the fixed position <h1'> element is sitting.
2- **z-index**
When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the elements that appear later in the
HTML code sits on top of those that are earlier on the page.
If you want to control which element sits on top, you can use
the z-index property. Its value is a number, and the higher the
number the closer that element is to the front. For example, an
element with a z-index of 10 will appear over the top of one
with a z-index of 5.
This example looks similar to the one on page 368, but it uses relative positioning for the <'p> elements. Because the paragraphs are relatively positioned, by default they would appear over the top of the
heading as the user scrolls down the page. To ensure that the
<'h1> element stays on top, we use the z-index property on the
rule for the <'h1> element. The z-index is sometimes referred to as the stacking context (as if the blocks have been stacked on top of each
other on a z-axis). If you are familiar with desktop publishing
packages, it is the equivalent of using the 'bring to front' and
'send to back' features
* **Floating Elements**
Floating an element allows you to take that element out of the normal flow and position it to the far left or right of a containing box. They floated element becomes a block-level element around which other content can flow
1- **float**
The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible. Anything else that sits inside the containing element will
flow around the element that is floated.When you use the float
property, you should also use the width property to indicate how
wide the floated element should be. If you do not, results can be
inconsistent but the box is likely to take up the full width of the
containing element (just like it would in normal flow).
In this example, a <'blockquote> element is used to hold a quotation. It's containing element is the <'body> element. The <'blockquote> element is floated to the right, and the paragraphs that follow the quote flow around the floated element.
