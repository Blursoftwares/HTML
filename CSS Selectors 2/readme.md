# Selectors part 2
***This is a continuation of the selectors section***

## ID and Class Selectors
ID selectors pick all components with a specific ID attribute value. In CSS, we express an ID selector by following the element name with a hash symbol and then the ID attribute value we want to match. In this scenario, the browser looks for a p element with the ID "introduction" and applies the CSS to it.
```css
p#introduction {
  color: blue;
}
```
```html
<p id="introduction">I'm blue</p>
```
ID selectors are useful when you want to give a single element on the page a unique identity and set it apart from everything else.

## Compound Selectors
Compound selectors let us apply the same CSS rules to multiple elements at once. 
If we want to make both `h2` and `h3` elements display green, we use both as selectors, separated with a comma.

```css
h2,
h3 {
  color: green;
}
```
```html
<h2>I'm green</h2>
<h3>I'm green too</h3>
<h4>I'm not green</h4>
```
This eliminates the need to rewrite a new CSS rule containing the same styles for different elements.

## Descendant Selectors
Descendant selectors choose components that are descendants of the matched selection name. A space between selectors indicates a descendant selector.

```html
article p {
  color: blue;
}
```
In this case, only `p` elements within the article element will receive the styling.

```html
<article>
  <p>I'm blue</p>
</article>

<p>I'm not blue</p>
```

## Adjacent Sibling Selector
The adjacent sibling selector targets elements that appear directly after the matching selector name. We indicate it using a plus symbol.

```css
h3 + p {
  color: blue;
}
```
The nearby sibling selector will style the paragraph immediately after the `h3` element, but not paragraphs that follow after it.
```html
<h3>Header</h3>
<p>I'm blue</p>
<p>I'm not blue</p>
```

## General Sibling Selector
The generic sibling selector (also known as the preceded selector) styles all matched items following the preceding selection name.
```css
h3 ~ p {
  color: pink;
}
```
With this general sibling selector, all paragraph elements that come after the `h3` will receive the styling.

```html
<h3>Header</h3>
<p>I'm pink</p>
<p>I'm pink</p>
```

## Universal Selector
The universal selector matches any elements and will apply to elements that are not targeted by other rules. It's indicated by the star symbol.

```css
* {
  color: yellow;
}
```
In this case, this is going to set the color of the text yellow for any element that hasn't had its color property specified elsewhere.
```html
<h2>I'm yellow</h2>

<p>I'm yellow</p>

<div>I'm yellow</div>
```

## Attribute Selectors
Attribute selectors** let you style elements based on their **HTML attributes**. Think of it like saying, "I want to style all toys (HTML elements) that have a specific tag (attribute) on them!"

This selects any HTML element with a specific **attribute and value**. For example, let’s style all `<input>` elements with the attribute `type="text"`.

```html
<!-- HTML Code -->
<input type="text" value="Name">
<input type="checkbox">

```
```css
input[type="text"] {
  background-color: lightblue;
}
```
The `[type="text"]` selector styles all input elements that have `type="text"`, making their background color light blue.

>[!note]
>Attribute selectors are like finding toys with specific tags and styling them!

## Pseudo-selectors

Pseudo-selectors let you style elements based on their state or position on the page. Think of it like saying, "I want to style this toy, but only when it’s being used or in a special place!"
There are two main types of pseudo-selectors:

* Pseudo-classes: These target elements in a special state (like when a button is hovered over).
* Pseudo-elements: These target specific parts of an element (like the first letter of a paragraph).

Let's look at how both look like.

**Pseudo-class**
The :hover pseudo-class styles an element when you move your mouse over it.

```html
<button>Hover over me!</button>
```
The :hover pseudo-class changes the button's background to yellow when you hover over it with your mouse.

```css
button:hover {
  background-color: yellow;
}
```
Hovering over the button will turn it yellow.

**Pseudo-elements**

The ::first-letter pseudo-element lets you style the first letter of a paragraph differently from the rest of the text. For elements, we use two colons.

```html
<p>This is a special paragraph.</p>
```
```css
p::first-letter {
  font-size: 30px;
  color: red;
}
```
Explanation: The `::first-letter` pseudo-element makes the first letter of the paragraph larger and red.













 
