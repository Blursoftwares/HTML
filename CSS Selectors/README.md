# CSS Selectors

## Objectives
- **What is a Selector?**
- **Selector Lists**
- **Types of Selectors**

## Introduction

**CSS selectors** help us choose which HTML elements we want to **style**. Imagine them as **magnifying glasses** that let us point to different toys (HTML elements) in our toy room (webpage) and say, "I want to color that!"

In this lesson, we’ll explore:
- What **selectors** are.
- **Different types** of selectors.
- How to use them in **CSS code**.

>[!note]
>Selectors are like **pointing** at something you want to decorate on your webpage!

---

## What is a Selector?

A **selector** is like telling CSS, "Hey, I want to style this part of my webpage!" Once you point at something (an HTML element), you can give it **rules** like color, size, and position.

Here’s an example:

```html
<!-- HTML Code -->
<p>This is a paragraph.</p>
```
```css


p {
  color: blue;
}
```

The `p` in CSS is a selector. It selects all the `<p>` elements (paragraphs) and turns them blue.

## Selector Lists

Sometimes, we want to style more than one type of HTML element at once. We can do that by using a selector list. This means we put multiple selectors together, separated by commas.
For instance;
```html
<h1>This is a heading</h1>
<p>This is a paragraph</p>
```
```CSS
h1, p {
  color: green;
}
```
The `h1, p` selects both the `<h1>` and `<p>` elements and makes them green.

## Types of Selectors
There are many different types of CSS selectors! Here are some of the most common:

### 1. Element Selector

This selector picks all elements of a certain type. For example, you can style every paragraph on the page.

Example:
```html

<p>Paragraph 1</p>
<p>Paragraph 2</p>
```
```css
p {
  color: red;
}
```
The `p` selector turns all paragraphs on the page red.


### 2. Class Selector
A class selector is used when we want to style a group of elements. It’s like saying, "All toys with a red tag should be blue."
For example;

```html

<p class="special">I am special!</p>
<p>I am not special.</p>

```
```css
.special {
  color: blue;
}
```
Explanation: The `.special` selector targets any HTML element with the class `special` and turns it blue.Additionally, since it is in 
the `<p>` tag, you can use `p.special`, try it!

### 3. ID Selector
An ID selector is for one unique element on the page. It's like saying, "Only this toy with the star sticker should look different."
For example;

```html
<p id="unique">I am unique!</p>
<p>I am not unique.</p>
```
```css
#unique {
  color: purple;
}
```
The `#unique` selector targets the element with the ID `unique` and makes it purple.

## Summary
* Selectors are used to choose which parts of your webpage to style.
* We can use element selectors to style all of one type, like all paragraphs.
* Class selectors let us style a group of elements that share the same class.
* ID selectors target just one special element on the page.
* Selector lists help us style more than one thing at once!

Now you're ready to start selecting and styling parts of your webpage with CSS!
