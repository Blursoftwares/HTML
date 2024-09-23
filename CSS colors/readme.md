# Various Types of Color Values in CSS

## Objectives
* How are colors displayed in CSS
* What are Hexadecimal values
* What are RGB  values
* What are comments?



When writing CSS, there are **different ways** to define colors beyond using simple color names like "red" or "blue." Let's explore some of these **color value types**, such as **hexadecimal**, **RGB**, and **RGBA** values, along with how to use **CSS comments**.

---

## Hexadecimal Color Values

**Hexadecimal colors** are a popular way of specifying colors in CSS. These colors start with a `#` followed by **6 characters**, which can be **numbers (0-9)** or **letters (a-f)**. The letters represent numbers in **hexadecimal (base 16)**.

### Example:

```css

p {
  color: #000000; 
}


p {
  color: #ffffff; 
}
```
`#000000` means no red, no green, no blue, which creates black.
`ffffff` means the maximum value of red, green, and blue, creating white.

## How Hex Colors Work

Hex colors represent values for Red (R), Green (G), and Blue (B). For example, the color red would be:
```css
p {
  color: #ff0000; 
}
```
#ff0000  means:
* ff for full red,
* 00 for no green,
* 00 for no blue.

**Shortened Hex Colors**
You can shorten a hex color when each of the digits repeats. For example:
```css
p {
  color: #111; 
}
```
`#111` is a shorthand for `#111111`, a dark gray color.

## RGB Color Values
RGB values let you set colors using numbers from 0 to 255 to represent the intensity of Red, Green, and Blue. The syntax looks like this:

```css
p {
  color: rgb(255, 0, 0); /* This is red */
}
```
* The first number is for Red (255 is the maximum amount of red),
* The second number is for Green (0 means no green),
* The third number is for Blue (0 means no blue).

## CSS Comments
CSS comments are helpful when you want to add notes or explanations in your code. These comments won't affect how your page looks because browsers ignore them.

```css
/* This paragraph is styled with a red alert color */
p.alert {
  color: #ff0000; /* Alert text displays red */
}
```
Everything inside the `/*`` */` is a comment. It's meant for other developers to understand the code but doesn't show up on the webpage.
>[!note]
>Use comments to explain your code, especially when it might be unclear for others or for future reference!

It's game time, check out our [Dinner Table](https://flukeout.github.io/)

## Resources
* [Tuts 30 Selectors](https://webdesign.tutsplus.com/the-30-css-selectors-you-must-memorize--net-16048t)
* [MDN CSS Tutorials for beginners](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps)
