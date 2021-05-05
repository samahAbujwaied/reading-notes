# Forms
![](https://bashooka.com/wp-content/uploads/2018/10/js-form-2018-1.jpg)

* How to collect information from visitors
* Different kinds of form controls
* New HTML5 form controls

# Why Forms?
*The best known form on the web is probably the search box that sits right in the middle of Google's homepage.*
*In addition to enabling users to search, forms also allow users to perform other functions online. You will see forms*
*when registering as a member of a website, when shopping online, and when signing up for newsletters or mailing lists.*

## Form Controls
* Adding text
> 1. Text input (single line)
  2. Pasword input 
  3. Text area 
![](https://cdn-media-1.freecodecamp.org/images/1*7dd2MZ78ekF3bA3N0Jlvmw.gif)

* Making Choices 
> 1. Radio buttons
  2. Checkboxes 
  3. Drop-down boxes 
![](https://kyusuf.com/images/css-forms/thumbnail.png)

# How forms work 
1. A user fills in a form and then presses a button to submit the information to the server.
2. The name of each form control is sent to the server along with the value the user enters or selects.
3. The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database.
4.The server creates a new page to send back to the browser based on the information received.

![](https://slideplayer.com/slide/15650516/88/images/4/What+happened+when+forms+were+submitted.jpg)

![](https://image.slidesharecdn.com/lesson7cssforms-181121231142/95/lesson-7-css-forms-7-638.jpg?cb=1542842074)

# Form structure 
* form every form tag requires an action attribute its value is the URL for the page on the server that will receive the information in the form when it is submitte.
* method Forms can be sent using one of two methods: get or post.

![](https://www.seoblog.com/wp-content/uploads/2018/02/Get-vs-Post.jpg)

## Text input 
* input tag has type attribute has a value 'text' its ceate a single line text input.
* name 
* size 
* maxlength 

## Password input
* input tag has a type attribute that has a 'password' it creates a text box that acts just like a single-line text input, except the characters are blocked out. They are hidden in this way so that if someone is looking over the user's shoulder, they cannot see sensitive data such as passwords.
* name 
* size 
* maxlenght

## Text area
* The ```<textarea>``` element
is used to create a mutli-line
text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag. Any text that appears between the opening ```<textarea>``` and closing ```</textarea> ```tags will appear in the text box when the page loads.

## Radio button 
* ```<input> ```type="radio" Radio buttons allow users to pick just one of a number of options.
* name The name attribute is sent to the server with the value of the option the user selects. When
a question provides users with options for answers in the form of radio buttons, the value of the name attribute should be the same for all of the radio buttons used to answer that question.
* size 
* maxlenght

## Checkbox
* ```<input>``` type="checkbox" Checkboxes allow users to select (and unselect) one or more options in answer to a question.
* name 
* size 
* maxlenght

## Drop Down list box
* ```<select>``` A drop down list box (also known as a select box) allows users to select one option from a drop down list The ```<select>``` element is used to create a drop down list box. It contains two or more ```<option>``` elements.
* ```<option>``` The ```<o ption>``` element is used to specify the options that the user can select from. The words between the opening ```<option> ```and closing ```</option> ```tags will be shown to the user in the drop down box.

# Submit button
* ```<input> ```type="submit" The submit button is used to send a form to the server.
* name It can use a name attribute but it does not need to have one.
value
* The value attribute is used to control the text that appears
on a button. It is a good idea to specify the words you want to appear on a button because the default value of buttons on some browsers is ‘Submit query’ and this might not be appropriate for all kinds of form.

## Image button
* ```<input>```type="image" If you want to use an image for the submit button, you can give the type attribute a value of image. The src, width, height, and alt attributes work just
like they do when used with the ```<img>`` element (which we saw on pages 99-100).

# html5: Form Validation
**You have probably seen forms on the web that give users messages if the form control has not been filled in correctly; this is known as form validation.Traditionally, form validation has been performed using JavaScript (which is beyond the scope of this book). But HTML5 is introducing validation and leaving the work to the browser.**

# html5: data input 
**```<input>```Many forms need to gather information such as dates, email addresses, and URLs. This has traditionally been done using text inputs.**
**type="date"If you are asking the user for a date, you can use an ```<input>``` element and give the type attribute a value of date.This will create a date input in browsers that support the new HMTL5 input types.**

# Lists, tables and Forms
* Specifying bullet point styles
* Adding borders and backgrounds to tables
* Changing the appearance of form elements

1. Bullet point styles
2. images for bullets 
3. positioning the marker 
4. list shorthand
5. table properties 
6. borderon empty cells 
7. GAOs between cells

## Styling submit buttons
![](https://freefrontend.com/assets/img/css-submit-buttons/CSS-Button-Interaction.gif)

## styling fieldsets & Legends
![](https://i.stack.imgur.com/2Ce2d.png)

## Aligning form controls : problem 
![](https://i.stack.imgur.com/QjzGM.png)

## Aligning form controls : solution 
![](https://www.formsite.com/wp-content/uploads/2017/04/formsite-align-left.png)

## Cursor styles 
![](https://lh3.googleusercontent.com/proxy/1oSiSG456gFZqM7u9zR73vbwR80N8ghdWkhFSOb7Gko5YpZNKxVSM8-tqKk3-2ASdbvsuLTbuGduxvyfRT3ZMZ7S7pFAdk1V4NdP2w)

# Events in JS
* Different event types
![](https://slidetodoc.com/presentation_image/136f5d765d0686d925d0c3c7e2c96a57/image-15.jpg)
![](https://slidetodoc.com/presentation_image/136f5d765d0686d925d0c3c7e2c96a57/image-16.jpg)
![](https://slidetodoc.com/presentation_image/136f5d765d0686d925d0c3c7e2c96a57/image-17.jpg)
![](https://slidetodoc.com/presentation_image/136f5d765d0686d925d0c3c7e2c96a57/image-18.jpg)
![](https://slidetodoc.com/presentation_image/136f5d765d0686d925d0c3c7e2c96a57/image-19.jpg)

#  HOW EVENTS TRIGGER JAVASCRIPT CODE 
![](https://slidetodoc.com/presentation_image/136f5d765d0686d925d0c3c7e2c96a57/image-14.jpg)
# HTML EVENT HANDLER ATTRIBUTES (DO NOT USE)
![](https://s3.ap-south-1.amazonaws.com/s3.studytonight.com/tutorials/uploads/pictures/1589352735-1.png)
#  TRADITIONAL DOM EVENT HANDLERS 
![](https://slidetodoc.com/presentation_image/136f5d765d0686d925d0c3c7e2c96a57/image-34.jpg)

# USING DOM EVENT HANDLERS
![](https://bennadel-cdn.com/resources/uploads/jquery_event_binding_on_detached_dom_nodes.jpg)

#  USING PARAMETERS WITH EVENT LISTENERS
![](https://i.stack.imgur.com/9syRo.png)

#  USING EVENT LISTENERS WITH THE EVENT OBJECT
![](https://docs.oracle.com/javase/tutorial/figures/uiswing/events/2eventsource.gif)

