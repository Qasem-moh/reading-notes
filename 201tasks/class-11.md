# Images

## Controlling sizes of Article images in CSS

_You can control the size of an image using the width and height properties in CSS, just like you can for any other box._

_Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download._

_You might think that your site is likely to have images of all different sizes, but a lot of sites use the same sized image across many of their pages._

_For example, an e-commerce site tends to show product photos at the same size. Or, if your site is designed on a grid, then you might have a selection of image sizes that are commonly used on all pages, such as:_
_Small portrait: 220 x 360_
_Small landscape: 330 x 210_
_Feature photo: 620 x 400_
_Whenever you use consistently_
_sized images across a site, you can use CSS to control the dimensions of the images, instead of putting the dimensions in the HTML._

## Aligning images Article Using CSS

_In the last chapter, you saw how the float property can be used to move an element to the left or the right of its containing block, allowing text to flow around it. Rather than using the <'img>_
_element's aligned attribute, web page authors are increasingly_
_using the float property to align images. There are two ways that_
_this is commonly achieved:_
_1: The float property is added to the class that was created to represent the size of the image (such as the small class in our example)._
_2: New classes are created with names such as align-left or_
_align-right to align the images to the left or right of the page._
_These class names are used in addition to classes that indicate the size of the image._

## Centering Article images Using CSS

_By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a block-level element using the display property with a value of the block._

_Once it has been made into a block-level element, there are_
_two common ways in which you can horizontally center an_ _image:_
_1: On the containing element,you can use the text-align property with a value of center._
_2: On the image itself, you canuse the margin property_
_and set the values of the left andright margins to auto._
_You can specify class namesthat allows any element to be_
_centered, in the same way, that you can for the dimension_

## Background Images

**background-image**

_The background-image property allows you to place_
_an image behind any HTML element. This could be the entire_
_page or just part of the page. By default, a background_ _image will repeat to fill the entire box._

## Repeating Article Images

**background-repeat**
**background-attachment**
_The background-repeat property can have four values:_
_**repeat** The background image is repeated both horizontally_ _and vertically (the default way it is shown if the background-repeat property isn't used)._
**repeat-x**
_The image is repeated horizontally only (as shown in_
_the first example on the left)._
**repeat-y**
_The image is repeated vertically only._
**no-repeat**
_The image is only shown once.The background-attachment_
_property specifies whether a background image should stay in_
_one position or move as the user scrolls up and down the page. It can have one of two values:_
**fixed**
_The background image stays in the same position on the page._
_scroll The background image moves up and down as the user scrolls up and down the page._

***
