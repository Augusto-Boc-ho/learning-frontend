# step 1

In this project, you will learn the basics of CSS (Cascading Style Sheets) by building a cafe menu. CSS is the language used to style an HTML document. It describes how HTML elements should be displayed on the screen.

As you learned in the last few steps of the Cat Photo App, there is a basic structure needed to start building your web page. Every HTML document should have a DOCTYPE declaration and html element. The DOCTYPE tells the browser which version of HTML the document is in. And the html element represents the root element which contains all other elements.
Example Code

<!DOCTYPE html>
<html lang="en">
<!--all other elements go here-->
</html>

# step 2

head with title

# step 3

Adding meta tags with utf-8

# step 4

Adding a body element

# step 5

Adding a main element which eventually will contains the menu information

# step 6

Adding an h1 with the title

# step 7

Adding a p

# step 8

Adding a section inside the main element

# step 9

Adding an h2

# step 10

Up until now, you have been limited regarding the presentation and appearance of the content you create. To start taking control, add a style element within the head element.

# step 11

You can add style to an element by specifying it in the style element and setting a property for it like this:
Example Code

element {
property: value;
}

Center the content of the h1 element by setting its text-align property to the value center.

# step 12

In the previous step, you used a type selector to style the h1 element. Center the content of the h2 and the p elements by adding a new type selector for each one to the existing style element.

# step 13

You now have three type selectors with the exact same styling. You can add the same group of styles to many elements by creating a list of selectors. Each selector is separated with commas like this:
Example Code

selector1, selector2 {
property: value;
}

Delete the three existing type selectors and replace them with one selector list that centers the text for the h1, h2, and p elements.

# step 14

You have styled three elements by writing CSS inside the style tags. This works, but since there will be many more styles, it's best to put all the styles in a separate file and link to it.

We have created a separate styles.css file for you and switched the editor view to that file. You can change between files with the tabs at the top of the editor.

Start by rewriting the styles you have created into the styles.css file. Make sure to exclude the opening and closing style tags.

# step 15

Now that you have the CSS in the styles.css file, go ahead and remove the style element and all its content. Once it is removed, the text that was centered will shift back to the left.

# step 16

Now you need to link the styles.css file, so the styles will be applied again. Inside the head element, add a link element. Give it a rel attribute with the value of "stylesheet" and an href attribute with the value of "styles.css".

# step 17

For the styling of the page to look similar on mobile as it does on a desktop or laptop, you need to add a meta element with a special content attribute.

Add the following within the head element:
Example Code

<meta name="viewport" content="width=device-width, initial-scale=1.0" />

# step 18

The text is centered again so the link to the CSS file is working. Add another style to the file that changes the background-color property to brown for the body element.

# step 19

changing the color another time

# step 20

The div element is used mainly for design layout purposes unlike the other content elements you have used so far. Add a div element inside the body element and then move all the other elements inside the new div.

Inside the opening div tag, add the id attribute with a value of menu.

# step 21

The goal now is to make the div not take up the entire width of the page. The CSS width property is perfect for this.

You can use the id selector to target a specific element with an id attribute. An id selector is defined by placing the hash symbol # directly in front of the element's id value. For example, if an element has the id of cat then you would target that element like this:
Example Code

#cat {
width: 250px;
}

# step 22

Comments in CSS look like this:
Example Code

/_ comment here _/

In your style sheet, comment out the line containing the background-color property and value, so you can see the effect of only styling the #menu element. This will make the background white again.

# step 23

Now use the existing #menu selector to set the background color of the div element to be burlywood.

# step 24

Now it's easy to see that the text is centered inside the #menu element. Currently, the width of the #menu element is specified in pixels (px).

Change the width property's value to be 80%, to make it 80% the width of its parent element (body).

# step 25

Next, you want to center the #menu horizontally. You can do this by setting its margin-left and margin-right properties to auto. Think of the margin as invisible space around an element. Using these two margin properties, center the #menu element within the body element.

# step 26

So far you have been using type and id selectors to style elements. However, it is more common to use a different selector to style your elements.

A class selector is defined by a name with a dot directly in front of it, like this:
Example Code

.class-name {
styles
}

Change the existing #menu selector into a class selector by replacing #menu with a class named .menu.

# step 27

To apply the class's styling to the div element, remove the id attribute and add a class attribute to the div element's opening tag. Make sure to set the class value to menu.

# step 28

Since the cafe's main product for sale is coffee, you could use an image of coffee beans for the background of the page.

Delete the comment and its contents inside the body type selector. Now add a background-image property and set its value to url(https://cdn.freecodecamp.org/curriculum/css-cafe/beans.jpg).

# step 29

It’s looking good. Time to start adding some menu items. Add an empty article element under the Coffee heading. It will contain a flavor and price of each coffee you currently offer.

# step 30

article elements commonly contain multiple elements that have related information. In this case, it will contain a coffee flavor and a price for that flavor. Nest two p elements inside your article element. The first one's text should be French Vanilla, and the second's text 3.00.

# step 31

Starting below the existing coffee/price pair, add the following coffee and prices using article elements with two nested p elements inside each. As before, the first p element's text should contain the coffee flavor and the second p element's text should contain the price.
Example Code

Caramel Macchiato 3.75
Pumpkin Spice 3.50
Hazelnut 4.00
Mocha 4.50

# step 32

The flavors and prices are currently stacked on top of each other and centered with their respective p elements. It would be nice if the flavor was on the left and the price was on the right.

Add the class name flavor to the French Vanilla p element.

# step 33

Using your new flavor class as a selector, set the text-align property's value to left.

# step 34

Next, you want to align the price to the right. Add a class named price to your p element that has 3.00 as its text.

# step 35

Now align the text to the right for the elements with the price class.

# step 36

That is kind of what you want, but now it would be nice if the flavor and price were on the same line. p elements are block-level elements, so they take up the entire width of their parent element.

To get them on the same line, you need to apply some styling to the p elements so they behave more like inline elements. To do that, start by adding a class attribute with the value item to the first article element under the Coffee heading.

# step 37

The p elements are nested in an article element with the class attribute of item. You can style all the p elements nested anywhere in elements with a class named item like this:
Example Code

.item p { }

Using the above selector, add a display property with value inline-block so the p elements behave more like inline elements.

# step 38

That's closer, but the price didn't stay over on the right. This is because inline-block elements only take up the width of their content. To spread them out, add a width property to the flavor and price class selectors that have a value of 50% each.

# step 39

Well that did not work. Styling the p elements as inline-block and placing them on separate lines in the code creates an extra space to the right of the first p element, causing the second one to shift to the next line. White space characters can cause this issue as well.

One way to fix this is to make each p element's width a little less than 50%. Change the width value to 49% for each class to see what happens.

# step 40

You could keep trying various percentages for the widths. Instead, use the back space key on your keyboard to move the p element with the class price next to the p element with the class flavor so that they are on the same line in the editor. Make sure there is no space between the two elements.

# step 41

Now go ahead and change both the flavor and price class' widths to be 50% again.

# step 42

Now that you know it works, you can change the remaining article and p elements to match the first set. Start by adding the class item to the other article elements.

# step 43

Next, position the other p elements to be on the same line with no space between them.

# step 44

To complete the styling, add the applicable class names flavor and price to all the remaining p elements.

# step 45

If you make the width of the page preview smaller, you will notice at some point, some of the text on the left starts wrapping around to the next line. This is because the width of the p elements on the left side can only take up 50% of the space.

Since you know the prices on the right have significantly fewer characters, change the flavor class width value to be 75% and the price class width value to be 25%.

# step 46

# step 47

# step 48

# step 49

# step 50

# step 51

# step 52

# step 53

# step 54

# step 55

# step 56

# step 57

# step 58

# step 59

# step 60

# step 61

# step 62

# step 63

# step 64

# step 65

# step 66

# step 67

# step 68

# step 69

# step 70

# step 71

# step 72

# step 73

# step 74

# step 75

# step 76

# step 77

# step 78

# step 79

# step 80

# step 81

# step 82

# step 83

# step 84

# step 85

# step 86

# step 87

# step 88

# step 89

# step 90

# step 91
