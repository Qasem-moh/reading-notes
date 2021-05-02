# What's a Table?

_A table represents information in a grid format._

_HTML tables allow web developers to arrange data into rows and columns. Grids allow us to understand complex data by referencing information on two axes. Each block in the grid is referred to as a table cell. In HTML a table is written out row by row._

![table](https://www.blog.duomly.com/wp-content/uploads/2020/05/basic-table-structure-c.png)

## Basic Table Structure

_At their most basic, tables are made up cells, arranged into rows and columns. You can control display characteristics for the whole table level, the row level, and for individual cells (there are currently no supported methods for controlling columns as a group)._

_The bare minimum tags for describing a table are <table'>, <tr'>, and <td'>. The following HTML shows the basic structure for a four-cell table:_

![Table Structure](https://learnerszonehome.files.wordpress.com/2019/07/html_table_structure.gif)

## Table Headings

_A table header is a row at the top of a table used to label each column. For example, in the below table there are three columns with a "Name," "Date of Birth," and "Phone" header._

![Headings](https://i.ibb.co/6rwHR5h/22.png)

## Spanning ColumnS

_To cause an item to span across columns use the property column-span with a value of all. This will cause the element to span all of the columns._

**example**

![](https://i.ibb.co/T1MxDwm/2021-05-02-23-14.png)

**result**

![](http://i.stack.imgur.com/voMBJ.jpg)

## Long Tables

_There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content). These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table (as you will see when you learn about CSS)._

**<thead'>: The Table Head element**

_The headings of the table should sit inside the <thead'> element._

![thead](https://cdn.educba.com/academy/wp-content/uploads/2020/02/THead-Tag-in-HTML.jpg)

**<tbody'>: The Table Body element**

_HTML <tbody'> tag is used to group the table rows (<tr'>) together, which indicates that this is body part of a table (<table'>)._

_The <tbody'> tag must be a child of <table'> element._

_The <tbody'> is used along with <thead'> and <tfoot'> which shows the different part of the table that are table head, table body, and table footer, however, it does not affect the layout of the table._

_These elements can be used for providing semantic information which can be helpful in accessibility purpose, or rendering the header at top and footer at the bottom while printing a large table._

---

## Width & Spacing

_To set the table width in HTML, use the style attribute. The style attribute specifies an inline style for an element. The attribute is used with the HTML <table'> tag, with the CSS property width. HTML5 do not support the width attribute of <table'>, so the CSS property width is used with the style attribute to set table width._

![](https://www.tutorialspoint.com/assets/questions/images/112715-1516259472.jpg)

_The HTML <table'> cellspacing Attribute is used to specify the space between the cells. The cellspacing attribute is set in terms of pixels._
![](https://media.geeksforgeeks.org/wp-content/uploads/20190529000101/cellsp.jpg)

## Border & Background

In HTML, there are two ways of adding a border to your tables. The first is to use the HTML border attribute. The other is to use CSS.

**HTML Table Border**

You can get a quick border around your table by using the HTML border attribute. You determine the width of the border using a number. For example, for a thin border, use the number "1". For a thicker border, use a greater number.

Like this:
![Border](https://i.ibb.co/3rzPMTn/2021-05-02-23-42.png)

---

# Function, Methods and Objects

_Browsers require very detailed instructions about what we want them to do. Therefore, complex scripts can run to hundreds (even thousands) of lines. Programmers use functions, methods, and objects to organize their code.This chapter is divided into three sections that introduce:_

**FUNCTIONS &METHODS OBJECTS**

_Functions consist of aseries of statements that have been grouped together because they perform a specific task. A method is the same as a function, except methods are created inside (and are part of) an object._

**OBJECTS**
_In Chapter 1 you saw that programmers use objects to create models of the worl d using data, and that objects are made up of properties and methods.In this secti on, you learn how to create your own objects using JavaScript._

**BUILT-IN OBJECTS**

_The browser comes with a set of objects that act like a toolkit for creating interactive web pages. This section introduces you to a number of built-in objects, which you will then see used throughout the rest of the book._

## WHAT IS A FUNCTI ON?

_Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than rep eating the same set of st atements)._

## A BASIC FUNCTION
![](https://miro.medium.com/max/654/1*suIOV93EyHolabBRpEXVIg.png)

_Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it._

**Function Declaration**

_To create a function we can use a function declaration._
_A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:_

_The name of the function._
_A list of parameters to the function, enclosed in arentheses and separated by commas.The JavaScript statements that define the function, enclosed in curly brackets, {...}._
![](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/declaration.svg)

**Function expression**
_The function keyword can be used to define a function inside an expression_

![](https://miro.medium.com/max/1492/1*_IejCVtnJg24RDNQC9xftg.png)

