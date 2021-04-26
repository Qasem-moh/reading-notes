# Lists

![Lists](https://i.ibb.co/6Rf5C32/download.jpg)

_There are lots of occasions when we need to use lists. HTML provides us with three different types:_

_HTML offers web authors three ways for specifying lists of information. All lists must contain one or more list elements. Lists may contain −_

_● Ordered lists are lists where each item in the list is numbered. For example, the list might be a set of steps fora recipe that must be performed in order, or a legal contract where each point needs to be identified by a section number._

_● Unordered lists are lists that begin with a bullet point (rather than characters that indicate order)._

_● Definition lists are made up of a set of terms along with the definitions for each of those terms._

![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2020/07/html-lists-df.jpg)

Ordered List /Numbered List (ol)​
The <ol'> tag is used to create an ordered list and <li'> tag starts the list of items. It is also called as a numbered list because list items are marked with numbers.



![](https://i.ibb.co/SdYJNgy/download-1.jpg)



***

A description list is a list of items with a description or definition of each item.

The description list is created using <dl> element. The <dl> element is used in conjunction with the <dt> element which specify a term, and the <dd> element which specify the term's definition.

Browsers usually render the definition lists by placing the terms and definitions in separate lines, where the term's definitions are slightly indented. Here's an example

![](https://www.wikitechy.com/step-by-step-html-tutorials/img/html-images/code-explanation-definition-list-dl-tag-in-html.png)
**Nested Article**

A nested list or a sublist is a list within a list. The trick to marking nested lists up correctly in HTML is to recognize that the sublist is actually a child of a list item and not of a list.

![](https://i.ibb.co/YydHMnV/4.png)



# Boxes
_At the beginning of this section on CSS, you saw how CSS treats each HTML element as if it lives in its own box._
_You can set several properties that affect the appearance of these boxes. In this chapter you will see how to:_

● Control the dimensions of your boxes
● Create borders around boxes
● Set margins and padding for boxes
● Show and hide boxes

_Once you have learned how to control the appearance of each box, you will see how to position these boxes on your pages in Chapter 15 when we look at page layout._

## Box Dimensions
**width, height** 
By default, a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the height and width properties. The most popular ways to specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size. When you use percentages, the size of the box is relative to the size of the browser window or, if the box is encased within another box, it is a percentage of the size of the containing box.
When you use ems, the size of the box is based on the size of the text within it. Designers have recently started to use percentages and ems more for measurements as they try to create designs that are flexible
across devices that have different-sized screens. In the example on the right, you can see that a containing <div> element is used which is 300 pixels wide by 300 pixels high. Inside of this is a paragraph that is 75% of the width and height of the containing element. This means that the size of the paragraph is 225 pixels wide by 225 pixels high.
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTSd_qmAi9A3oX-Ix4830CRI88VaVsFUHjL4rkBy0vzVq8WLCj5Eof3A4G4gE48nGP60fo&usqp=CAU)

**Limiting Article Width**
_min-width, max-width_

##  Min-Width And Max-Width Properties

_The first thing to discuss is width-related properties. We have min-width and max-width, and each one of them is important and has its use cases._

**Min Width**
When setting the value of min-width, its benefit lies in preventing the used value for width property from becoming less than the specified value for min-width. Note that the default value for min-width is auto, which resolves to 0.

Let’s take a basic example to demonstrate that.

![](https://ishadeed.com/assets/min-max/min-width-1.png)

We have a button with a varying text within in. The text might range from one word to multiple. To guarantee that it will have a minimum width even if it has one word only, min-width should be used. The minimum width is 100px so that even if the button has a very short content, like “Done” word, or an icon only, it will still be big enough to be noticed. This is very important when working with multilingual websites like Arabic. Consider the below example from Twitter:

![](https://ishadeed.com/assets/min-max/word-length-twitter.png)

_In the before case, the button has the word “تم”, which means Done. The button width is too small, so I increased the min-width of it as you notice in the after case._

## Min-Height And Max-Height Properties
_In addition to the minimum and maximum width properties, we have the same properties as the height._

**Min Height**

_When setting the value of min-height, its benefit lies in preventing the used value for height property from becoming less than the specified value for min-height. Note that the default value for min-height is auto, which resolves to 0._

_Let’s take an example to demonstrate a simple use case._

_We have a section with a description text. The goal is to have a minimum height for the section, so it can handle short or long content. Consider the below basic case:_

![](https://ishadeed.com/assets/min-max/min-height-1.png)

![](https://i.ibb.co/ZV3WqBg/Screenshot-from-2021-04-26-17-44-36.png)

_The minimum height is 100px, and with flexbox, the content is centered horizontally and vertically. What would happen if the content were longer? For example, a paragraph?_

![](https://ishadeed.com/assets/min-max/min-height-2.png)

_Yes, you guessed it! The height of the section will expand to contain the new content. By having that, we can build components that are fluid and responsive to its content._

***
**Max Height**
_When setting the value of max-height, its benefit lies in preventing the used value for height property from becoming more than the specified value for max-height. Note that the default value for max-height is none._

_Consider the below example where I set max-height for the content. But, because it’s bigger than the specified space, there is an overflow. The text is out of its parent boundaries due to that._

**ARRAYS**

_In JavaScript, array is a single variable that is used to store different elements. It is often used when we want to store list of elements and access them by a single variable. Unlike most languages where array is a reference to the multiple variable, in JavaScript array is a single variable that stores multiple elements._

_Declaration of an Array_
_There are basically two ways to declare an array._
_Example:_

**var House = [ ]; // method 1**
**var House = new array(); // method 2**

_But generally method 1 is preferred over the method 2. Let us understand the reason for this._
![](https://cdn-media-1.freecodecamp.org/images/w3CWlvnWqG5VEy6qupnAYvTqECGhPdj3P9Wu)
***
![](https://www.tutorialsteacher.com/Content/images/js/js-array.png)

**Array Initialization**
An array in JavaScript can be defined and initialized in two ways, array literal and Array constructor syntax.

**Array Literal**
Array literal syntax is simple. It takes a list of values separated by a comma and enclosed in square brackets.

var <'array-name'> = [element0, element1, element2,... elementN];

![](https://miro.medium.com/max/892/1*bFIR37BFmQcxyPd7UPs6xg.png)

_Let's look at by far the most common type of conditional statement you'll use in JavaScript — the humble if...else statement._

if (condition) {
  code to run if condition is true
} else {
  run some other code instead
}


Here we've got:

The keyword if followed by some parentheses.
A condition to test, placed inside the parentheses (typically "is this value bigger than this other value?", or "does this value exist?"). The condition makes use of the comparison operators we discussed in the last module and returns true or false.
A set of curly braces, inside which we have some code — this can be any code we like, and it only runs if the condition returns true.
The keyword else.
Another set of curly braces, inside which we have some more code — this can be any code we like, and it only runs if the condition is not true — or in other words, the condition is false.
This code is pretty human-readable — it is saying "if the condition returns true, run code A, else run code B"

You should note that you don't have to include the else and the second curly brace block — the following is also perfectly legal code:

if (condition) {
  code to run if condition is true
}

run some other code
However, you need to be careful here — in this case, the second block of code is not controlled by the conditional statement, so it always runs, regardless of whether the condition returns true or false. This is not necessarily a bad thing, but it might not be what you want — often you want to run one block of code or the other, not both.

_As a final point, you may sometimes see if...else statements written without the curly braces, in the following shorthand style:_

if (condition) code to run if condition is true
else run some other code instead
***

let shoppingDone = false;
let childsAllowance;

if (shoppingDone === true) {
  childsAllowance = 10;
} else {
  childsAllowance = 5;
}
***
**else if**

_The last example provided us with two choices, or outcomes — but what if we want more than two?_

_There is a way to chain on extra choices/outcomes to your if...else — using else if. Each extra choice requires an additional block to put in between if() { ... } and else { ... } :_
