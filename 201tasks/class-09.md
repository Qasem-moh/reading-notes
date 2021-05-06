# What's Form In HTML

_The HTML <'form> element represents a document section containing interactive controls for submitting information._

## HTML Form Elements

_HTML form elements are used to capture user input. There are many different types of form elements such as the text box, check box, drop down, submit button, and much more._

_Take a look at an example form with a few input elements below:_
![ELEMENTS](https://i.ibb.co/7RHYYj5/2021-05-06-22-57.png)

_The form elements above are the most common used form elements. We will go into further detail on each of these form elements:_

- **Text Box Input**
- **Password Input**
- **Text Area**
- **Select Drop Down**
- **Check Box**
- **Radio Input**
- **File Input**
- **Submit Button**

![form](https://i.ibb.co/3TNyRzz/4.png)

## Form Structure

**<'form>**
Form controls live inside a <'form> element. This element should always carry the action attribute and will usually have a method and id attribute too.

**action**
Every <'form> element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.

**method**
Forms can be sent using one of two methods: get or post.
With the get method, the values from the form are added to
the end of the URL specified in the action attribute.

- The get method is ideal for short forms (such as search boxes)

- when you are just retrieving data from the web server
  (not sending information that should be added to or deleted
  from a database) With the post method the values are sent in what are known as HTTP headers. As a rule of thumb you should use the post method if your form:
  1- allows users to upload a file
  2- is very long
  3- contains sensitive data
  (e.g. passwords)
  4- adds information to, or deletes information from, a database

If the method attribute is not used, the form data will be sent
using the get method.

**id**
We look at the id attribute on page 183, but the value is used to
identify the form distinctly from other elements on the page (and
is often used by scripts — such as those that check you have
entered information into fields that require values).

**Text Input**
The <input'> element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.

**type="text"**
When the type attribute has a value of text , it creates a single-line text input.

**name**
When users enter information into a form, the server needs to know which form control each piece of data was entered into. (For example, in a login form, the server needs to know what has been entered as the username and what has been given as the password.) Therefore, each form control requires a name attribute. The value of this attribute
identifies the form control and is sent along with the information they enter to the server.

**maxlength**
When users enter information into a form, the server needs to know which form control each piece of data was entered into. (For example, in a login form, the server needs to know what has been entered as the username and what has been given as the password.) Therefore, each form control requires a name attribute. The value of this attribute
identifies the form control and is sent along with the information they enter to the server.

**size**
The size attribute should not be used on new forms. It was
used in older forms to indicate the width of the text input
(measured by the number of characters that would be seen).
For example, a value of 3 would create a box wide enough to
display three characters.

**Password Input**

<'input>
type="password" When the type attribute has a value of password it creates a text box that acts just like a
single-line text input, except the characters are blocked out. They are hidden in this way so that if someone is looking over the user's shoulder, they cannot see sensitive data such as passwords.

**name**

The name attribute indicates the name of the password input, which is sent to the server with the password the user enters.

**size, maxlength**

It can also carry the size and maxlength attributes like the the single-line text input.

Although the password is hidden on the screen, this does not
mean that the data in a password control is sent securely to the
server. You should never use these for sending sensitive data
such as credit card numbers. For full security, the server needs
to be set up to communicate with users' browsers using
Secure Sockets Layer (SSL). The topic of SSL is beyond the scope
of this book, however there are links to learn more about it on
the accompanying website.

**Text AREA**
<'textarea>
The <'textarea> element is used to create a mutli-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag. Any text that appears between the opening <'textarea> and closing
<'/textarea> tags will appear in the text box when the
page loads.

**Radio Button**

<'input>
type="radio"
Radio buttons allow users to pick just one of a number of options.
**name**
The name attribute is sent to the server with the value of the
option the user selects. When a question provides users with
options for answers in the form of radio buttons, the value of
the name attribute should be the same for all of the radio buttons used to answer that question.

**value**
The value attribute indicates the value that is sent to  
server for the selected option. The value of each of the buttons
in a group should be different (so that the server knows which
option the user has selected).
**checked**
The checked attribute can be used to indicate which value (if
any) should be selected when the page loads. The value of this
attribute is checked . Only one radio button in a group should
use this attribute.

**Checkbox**

<'input>
type="checkbox"
Checkboxes allow users to select (and unselect) one or more
options in answer to a question.
**name**
The name attribute is sent to the server with the value of the
option(s) the user selects. When a question provides users with
options for answers in the form of checkboxes, the value of the
name attribute should be the same for all of the buttons that
answer that question.
**value**
The value attribute indicates the value sent to the server if this checkbox is checked.
**checked**
The checked attribute indicates that this box should be checked
when the page loads. If used, its value should be checked.

**Drop Down List Box**

<'select>
A drop down list box (also known as a select box) allows
users to select one option from a drop down list. The <'select> element is used to create a drop down list box. It contains two or more <'option> elements.
**name**
The name attribute indicates the name of the form control being
sent to the server, along with the value the user selected.
**<'option>**
The <'option> element is used to specify the options that the
user can select from. The words between the opening <'option>
and closing </option> tags will be shown to the user in the drop
down box.
**value**
The <'option> element uses the value attribute to indicate the
value that is sent to the server along with the name of the
control if this option is selected.

**selected**
The selected attribute can be used to indicate the option that
should be selected when the page loads. The value of this
attribute should be selected . If this attribute is not used,
the first option will be shown when the page loads. If the user
does not select an option, then the first item will be sent to
the server as the value for this control.
The function of the drop down list box is similar to that of the
radio buttons (in that only one option can be selected). There
are two key factors in choosing which to use:

1. If users need to see all options
   at a glance, radio buttons are
   better suited.

2. If there is a very long list
   of options (such as a list of
   countries), drop down list boxes
   work better.

**Multiple Select Box**
<'select>
**size**
You can turn a drop down select box into a box that shows more
than one option by adding the size attribute. Its value should
be the number of options you want to show at once. In the
example you can see that three of the four options are shown.
Unfortunately, the way that browsers have implemented this
attribute is not perfect, and it should be tested throroughly if
used (in particular in Firefox and Safari on a Mac).
**multiple**
You can allow users to select multiple options from this list by
adding the multiple attribute with a value of multiple .
It is a good idea to tell users if they can select more than one
option at a time. It is also helpful to indicate that on a PC they should hold down the control key while selecting multiple options and on a Mac they should use the command key while selecting options.
**File Input Box**

<'input>
If you want to allow users to upload a file (for example an
image, video, mp3, or a PDF), you will need to use a file input
box.
**type="file"**
This type of input creates a box that looks like a text input
followed by a browse button. When the user clicks on the
browse button, a window opens up that allows them to select a
file from their computer to be uploaded to the website.
When you are allowing users to upload files, the method
attribute on the <'form> element must have a value of post . (You
cannot send files using the HTTP get method.)
When a user clicks on the browse button, the presentation
of the window that allows them to browse for the file they
want to upload will match the windows of the user's operating
system. You cannot control the appearance of these windows

**Submit Button**

<'input>
**type="submit"**
The submit button is used to send a form to the server.
**name**
It can use a name attribute but it does not need to have one.
**value**
The value attribute is used to control the text that appears
on a button. It is a good idea to specify the words you want to
appear on a button because the default value of buttons on some
browsers is ‘Submit query’ and this might not be appropriate for
all kinds of form.
**Image Button**

<'input>
**type="image"**
If you want to use an image for the submit button, you can give
the type attribute a value of image . The src , width , height ,
and alt attributes work just like they do when used with the
<'img> element

**Button &hidden Controls**

**<'button>**

The <'button> element was introduced to allow users more
control over how their buttons appear, and to allow other
elements to appear inside the button. This means that you can combine text and images between the opening <'button>
tag and closing <'/button> tag.

**<'input>**

**type="hidden"**
This example also shows a hidden form control. These form
controls are not shown on the page (although you can see them
if you use the View Source option in the browser). They allow web
page authors to add values to forms that users cannot see.
For example, a web page author might use a hidden field to
indicate which page the user was on when they submitted a form.