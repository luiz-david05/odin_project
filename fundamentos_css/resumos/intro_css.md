## Basic Syntax

Css is made up varios rules. These rules are made up of a selectro and a semi-color separeted list of declarations , with each of those declarations being made up of a property: value pair;

```css
p {
    color: red;
    font-size: 20px;
}
```

## Selectors

Selectro simply refer to the HTML elements to wich CSS rule apply; they're what is actually being "selected" for each rule.


## Universal Selector

The universal selector, written as an asterisk (*), is essentially a way to target all elements in the document at once. It's often used to set default styles that are applied to all elements, such as removing the default margin and padding from all elements.

```css
* {
    margin: 0;
    padding: 0;
}
```

## Type Selector

A type selector (or element selector) will select all elements of given element type, and syntax is juts the name of the element:

```html
<div>Hello, World!</div>
<div>Hello again!</div>
<p>Hi...</p>
<div>Okay, bye.</div>
```

```css
div {
    color: red;
}
```

Here, all three <div> elements would be selected, while the <p> element wouldn’t be.


## Class Selector

A class selector will select all elements that have a given class attribute, and syntax is a period (.) followed by the class name:


```html
<div class="alert-text">Please agree to our terms of service.</div>
```

```css	
.alert-text {
  color: red;
}
```

Note the syntax for class selectors: a period immediately followed by the case-sensitive value of the class attribute. Classes aren’t required to be specific to a particular element, so you can use the same class on as many elements as you want.

Another thing you can do with the class attribute is to add multiple classes to a single element as a space-separated list, such as class="alert-text severe-alert". Since whitespace is used to separate class names like this, you should never use spaces for multi-worded names and should use a hyphen instead.


## ID Selector

ID selectors are similar to class selectors. They select an element with the given ID, which is another attribute you place on an HTML element. The major difference between classes and IDs is that an element can only have one ID. It cannot be repeated on a single page and should not contain any whitespace:

```html
<div id="title">My Awesome 90's Page</div>
```

```css
#title {
  background-color: red;
}
```