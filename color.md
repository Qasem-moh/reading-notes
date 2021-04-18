# Color in CSS
Color can really bring your pages to life.
In this chapter we will look at:

1. How to specify colors, as there are three common ways in
which you can indicate your choice of colors (plus extra
ways made available in CSS3)

2. Color terminology, as there are some terms that are very
helpful to understand when it comes to picking colors

3. Contrast, and ensuring that your text is readable

4. Background colors for behind either your entire page or
parts of a page

What you will learn about colors in this chapter will then be
used in subsequent chapters when it comes to looking at
colors of text and boxes in CSS.
***
The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:
## RGB values
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)
## HEX codes
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80
## color names
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan

We look at these three different
ways of specifying colors on the
next double-page spread.
CSS3 has also introduced
another way to specify colors
called HSLA, which you will
meet near the end of this chapter
on page 255-256.
Foreground Color
color
Above each CSS rule in this
example you can see how CSS
allows you to add comments
to your CSS files. Anything
between the /* symbols and
the */ symbols will not be
interpreted by the browser.
They are shown in grey above.
The use of comments can help
you to understand a CSS file
(and organise it, by splitting a
long document into sections).
Here, we have used comments
to indicate which method is used
to specify each of the different
types of colors
***
/* color name */
h1 {
color: DarkCyan;}
/* hex code */
h2 {
color: #ee3e80;}
/* rgb value */
p {
color: rgb(100,100,90);}
![](https://i.ibb.co/5shrdJJ/8.png)
***
## Background Color
#### background-color



_CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box. You can specify your choice of background color in the same three ways you can specify foreground colors: RGB values, hex codes, and color names (covered on the next page). If you do not specify a background color, then the background is transparent. By default, most browser windows have a white background, but browser users can set a background color for their windows, so if you want to be sure that the background
is white you can use the background-color property on the <body> element._
![](https://i.ibb.co/bHJb6Th/9.png)
![](https://i.ibb.co/tcDsbHS/10.png)

***
# Understanding Color
_Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, you can use a color picker._

_Computer monitors are made up of thousands of tiny squares called pixels (if you look very closely at your monitor you should be able to see them). When the screen is not turned on, it's black because it's not emitting any light. When it's
on, each pixel can be a different color, creating a picture. The color of every pixel on the screen is expressed in terms of a mix of red, green, and blue — just like on a television screen._
***
![](https://i.ibb.co/yWptNBQ/11.png)
_Color picking tools are available in image editing programs like Photoshop and GIMP. You can see the RGB values specified next to the radio buttons that
say R, G, B. The hex value is provided next to the pound or hash #symbol. There is also a good color picking tool at: colorschemedesigner.com_

![](https://i.ibb.co/jJ6kjhG/12.png)

## RGB Values
Values for red, green, and blue are expressed as numbers
between 0 and 255. rgb(102,205,170) This color is made up of the
following values:
**102 red**
**205 green**
**170 blue**
## Hex Codes
Hex values represent values for red, green, and blue in hexadecimal code
#66cdaa
The value of the red, 102, is expressed as 66 in hexadecimal code. The 205 of the green is expressed as cd and the 170 of
the blue equates to aa.
## Color Names
Colors are represented by predefined names. However, they are very limited in number.
MediumAquaMarine There are 147 color names supported by browsers (this color is MediumAquaMarine). Most consider this to be a limited color palette, and it is
hard to remember the name for each of the colors so (apart from white and black) they are not commonly used.

## Hue
Hue is near to the colloquial idea of color. Technically speaking however, a color can also have saturation and brightness as well as hue.
 
## Saturation
Saturation refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be mostly gray.
## Brigh tness
Brightness (or "value") refers to how much black is in a color.  At maximum brightness, there would be no black in the color. At minimum brightness, the
color would be very dark.