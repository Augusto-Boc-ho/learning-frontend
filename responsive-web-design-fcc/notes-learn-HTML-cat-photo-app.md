# step 1

HTML elements have opening tags like <h1> and closing tags like </h1>. The text an element will display goes between its opening and closing tags.

# step 2

The h1 through h6 heading elements are used to signify the importance of content below them. The lower the number, the higher the importance, so h2 elements have less importance than h1 elements.
Example Code

<h1>most important heading element</h1>
<h2>second most important heading element</h2>
<h3>third most important heading element</h3>
<h4>fourth most important heading element</h4>
<h5>fifth most important heading element</h5>
<h6>least important heading element</h6>

Only use one h1 element per page and place lower importance headings below higher importance headings.

# step 3

The p element is used to create a paragraph of text on websites.

# step 4

ommenting allows you to leave messages without affecting the browser display. It also allows you to make code inactive. A comment in HTML starts with <!--, contains any number of lines of text, and ends with -->.

Here is an example of a comment with the TODO: Remove h1:
Example Code

<!-- TODO: Remove h1 -->

# step 5

HTML5 has some elements that identify different content areas. These elements make your HTML easier to read and help with Search Engine Optimization (SEO) and accessibility.

The main element is used to represent the main content of the body of an HTML document. Content inside the main element should be unique to the document and should not be repeated in other parts of the document.
Example Code

<main>
  <h1>Most important content of the document</h1>
  <p>Some more important content...</p>
</main>

# step 6

In the previous step, you put the h1, h2, comment, and p elements inside the main element. This is called nesting. Nested elements should be placed two spaces further to the right of the element they are nested in. This spacing is called indentation and it is used to make HTML easier to read.

Here is an example of nesting and indentation:
Example Code

<main>
  <h1>Most important content of the document</h1>
  <p>Some more important content...</p>
</main>

# step 7

You can add images to your website by using the img element. img elements have an opening tag without a closing tag. An element without a closing tag is known as a void element.

# step 8

HTML attributes are special words used inside the opening tag of an element to control the element's behavior. The src attribute in an img element specifies the image's URL (where the image is located).

Here is an example of an img element with a src attribute pointing to the freeCodeCamp logo:
Example Code:
<img src="https://cdn.freecodecamp.org/platform/universal/fcc_secondary.svg">

# step 9

All img elements should have an alt attribute. The alt attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load.

Here is an example of an img element with an alt attribute:
Example Code

<img src="cat.jpg" alt="A cat">

# step 10

You can link to another page with the anchor (a) element.

Here is an example linking to https://www.freecodecamp.org:
Example Code

<a href="https://www.freecodecamp.org"></a>

# step 11

A link's text must be placed between the opening and closing tags of an anchor (a) element.

Here is an example of a link with the text click here to go to freeCodeCamp.org:
Example Code
<a href="https://www.freecodecamp.org">click here to go to freeCodeCamp.org</a>

# step 12

only added some words before and after the anchor element

# step 13

only was added the p element for the words that are around the anchor element

# step 14

Turn the existing text cute cats into an anchor element that links to:
https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg

# step 15

To open links in a new tab, you can use the target attribute on the anchor (a) element.

The target attribute specifies where to open the linked document. target="\_blank" opens the linked document in a new tab or window.

Here is the basic syntax for an a element with a target attribute:
Example Code
<a href="https://www.freecodecamp.org" target="_blank">freeCodeCamp</a>

# step 16

comment removed

# step 17

In previous steps you used an anchor element to turn text into a link. Other types of content can also be turned into a link by wrapping it in anchor tags.

Here is an example of turning an image into a link:
Example Code

<a href="example-link">
  <img src="image-link.jpg" alt="A photo of a cat.">
</a>

# step 18

Before adding any new content, you should make use of a section element to separate the cat photos content from the future content.

The section element is used to define sections in a document, such as chapters, headers, footers, or any other sections of the document. It is a semantic element that helps with SEO and accessibility.
Example Code

<section>
  <h2>Section Title</h2>
  <p>Section content...</p>
</section>

# step 19

adding a new section below the another one

# step 20

filling the new section

# step 21

adding an h3 element

# step 22

To create an unordered list of items, you can use the ul element.

# step 23

The li element is used to create a list item in an ordered or unordered list.

Here is an example of list items in an unordered list:
Example Code

<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>

# step 24

Adding a new photo with a link after the unordered list

# step 25

The figure element represents self-contained content and will allow you to associate an image with a caption.

# step 26

Step 26

A figure caption (figcaption) element is used to add a caption to describe the image contained within the figure element.

Here is an example of a figcaption element with the caption of A cute cat:
Example Code

<figure>
  <img src="image.jpg" alt="A description of the image">
  <figcaption>A cute cat</figcaption>
</figure>

# step 27

To place emphasis on a specific word or phrase, you can use the em element.

# step 28

Just adding another h3 element

# step 29

The code for an ordered list (ol) is similar to an unordered list, but list items in an ordered list are numbered when displayed.

# step 30

Adding a new figure element

# step 31

Adding an image inside the figure element

# step 32

Adding the alt attribute to the image

# step 33

Adding a figcaption to the image

# step 34

The strong element is used to indicate that some text is of strong importance or urgent.

# step 35

Adding a new section element

# step 36

Adding a new h2 element

# step 37

The form element is used to get information from a user like their name, email, and other details.

# step 38

The action attribute indicates where form data should be sent.

Here is an example of a form element with an action attribute:
Example Code

<form action="/submit-url"></form>

In the example, action="/submit-url" tells the browser that the form data should be sent to the path /submit-url.

# step 39

The input element allows you several ways to collect data from a web form. Like img elements, input elements are a void element and do not need closing tags.

# step 40

There are many kinds of inputs you can create using the type attribute. You can easily create a password field, reset button, or a control to let users select a file from their computer.

# step 41

In order for a form's data to be accessed by the location specified in the action attribute, you must give the text field a name attribute and assign it a value to represent the data being submitted.

Here is an example of an input element with a name attribute:
Example Code

<input type="text" name="name">

# step 42

Placeholder text is used to give people a hint about what kind of information to enter into an input.

Here is an example of an input element with a placeholder set to Ex. Jane Doe:
Example Code

<input type="text" placeholder="Ex. Jane Doe">

# step 43

To prevent a user from submitting your form when required information is missing, you need to add the required attribute to an input element. There's no need to set a value to the required attribute. Instead, just add the word required to the input element, making sure there is space between it and other attributes.

# step 44

The button element is used to create a clickable button.

# step 45

Even though you added your button below the text input, they appear next to each other on the page. That's because both input and button elements are inline elements, which don't appear on new lines.

The button you added will submit the form by default. However, relying on default behavior may cause confusion. Add the type attribute with the value submit to the button to make it clear that it is a submit button.

# step 46

You can use radio buttons for questions where you want only one answer out of multiple options.

Here is an example of a radio button with the text set as cat:
Example Code

<input type="radio"> cat

Remember that an input element is a void element.

# step 47

label elements are used to help associate the text for an input element with the input element itself (especially for assistive technologies like screen readers).

Here is an example of a label element with a radio button:
Example Code

<label><input type="radio"> cat</label>

In the example, clicking on the word "cat" will also select the radio button.

# step 48

The id attribute is used to identify specific HTML elements. Each id attribute's value must be unique from all other id values for the entire page.

Here is an example of an input element with an id attribute:
Example Code

<input id="email">

# step 49

Adding another button

# step 50

Notice that both radio buttons can be selected at the same time. To make it so selecting one radio button automatically deselects the other, both buttons must have a name attribute with the same value.

Here is an example of two radio buttons with the same name attribute:
Example Code

<input type="radio" name="meal"> Breakfast
<input type="radio" name="meal"> Lunch

# step 51

If you select the Indoor radio button and submit the form, the form data for the button is based on its name and value attributes. Since your radio buttons do not have a value attribute, the form data will include indoor-outdoor=on, which is not useful when you have multiple buttons.

# step 52

The fieldset element is used to group related inputs and labels together in a web form. fieldset elements are block-level elements, meaning that they appear on a new line.

# step 53

The legend element acts as a caption for the content in the fieldset element. It gives users context about what they should enter into that part of the form.

# step 54

Adding another fieldset element

# step 55

Adding another legend element

# step 56

Forms commonly use checkboxes for questions that may have more than one answer. The input element with a type attribute set to checkbox creates a checkbox.

# step 57

Adding an id value to the checkbox input

# step 58

Step 58

There's another way to associate an input element's text with the element itself. You can nest the text within a label element and add a for attribute with the same value as the input element's id attribute.

Given an input element as below:
Example Code

<input id="breakfast" type="radio" name="meal" value="breakfast">

An example of a label element that is associated to this input element is:
Example Code

<label for="breakfast">Breakfast</label>

# step 59

Adding a name to the checkbox input element

# step 60

While you won't notice this in the browser, doing this makes it easier for a server to process your web form, especially when there are multiple checkboxes.

Adding a new checkbox

# step 61

Adding another checkbox

# step 62

Adding value to the checkbox

# step 63

Step 63

In order to make a checkbox checked or radio button selected by default, you need to add the checked attribute to it.

Here is an example of a radio button with the checked attribute:
Example Code

<input checked type="radio" name="meal" value="breakfast"> Breakfast

There's no need to set a value to the checked attribute. Instead, just add the word checked to the input element, making sure there is space between it and other attributes.

# step 64

The footer element is used to define a footer for a document or section. A footer typically contains information about the author of the document, copyright data, links to terms of use, contact information, and more.

# step 65

Adding a p with copyright to the footer

# step 66

Turning some words of the p into a link

# step 67

Notice that everything you've added to the page so far is inside the body element. All page content elements that should be rendered to the page go inside the body element. However, other important information goes inside the head element.

The head element is used to contain metadata about the document, such as its title, links to stylesheets, and scripts. Metadata is information about the page that isn't displayed directly on the page.

And adding a head

# step 68

Adding a title

# step 69

Notice that the entire contents of the page are nested within an html element. The html element is the root element of an HTML page and wraps all content on the page.

You can also specify the language of your page by adding the lang attribute to the html element.

Add the lang attribute with the value en to the opening html tag to specify that the language of the page is English.

# step 70

All pages should begin with <!DOCTYPE html>. This special string is known as a declaration and ensures the browser tries to meet industry-wide specifications.

<!DOCTYPE html> tells browsers that the document is an HTML5 document which is the latest version of HTML.

Add this declaration as the first line of the code.

# step 71

You can set browser behavior by adding meta elements in the head. Here's an example:
Example Code

<meta attribute="value">

Inside the head element, nest a meta element with an attribute named charset. Set to the value to utf-8 which tells the browser how to encode characters for the page.

Note that the meta element is a void element.

With that last change, you have completed the Cat Photo App project. Congratulations!
