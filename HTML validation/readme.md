# HTML Validation

## Objectives

- **Identify W3C organization**: Learn about the organization that helps set the rules for writing valid HTML.
- **Validate sample HTML**: Discover how to use tools to check if our HTML is correct.
- **Identify HTML errors**: Learn how to spot common mistakes in HTML code and how to fix them.

## Introduction

You have written a few HTML pages by now. Did you accidentally break nesting and put emphasis on a whole page? Or did you type `<he>` instead of `<h3>`? How can we guard HTML? Many editors try to catch errors for us, and most browsers are pretty good at guessing what you meant. But what happens when Windows Edge guesses differently than Google Chrome? How can we be certain that our HTML meets standards and is error free? Luckily, the W3C – the people who define the tags of HTML – have a validation service we can use. We'll explain the W3C and their validator in this lesson.

## 1. What is W3C?

The **World Wide Web Consortium (W3C)** is a group that creates the rules and standards for writing HTML, CSS, and other web technologies. These standards help ensure that websites work the same way across all browsers.

### What Does W3C Do?
- They create rules for writing **valid HTML**.
- They ensure websites look and work correctly on all devices and browsers.
- They provide tools for checking if your HTML follows the correct rules.

To learn more about W3C, you can visit their [documentation](https://www.w3.org/)

## 2. Validating Sample HTML

### What is HTML Validation?

HTML validation is like having a teacher check your homework. It helps you make sure your HTML code is correct and follows all the rules. If there’s a mistake, the validator will point it out so you can fix it.

### 1. Using the W3C Validator

The W3C offers an **HTML Validator** tool. Here’s how to use it:
1. Go to the [W3C Validator](https://validator.w3.org/)
2. You can either paste your HTML code or provide the URL of your website.
3. The validator will check your HTML and show you any errors or warnings.

For this lesson, paste the following code;
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Valid HTML</title>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is a valid HTML page!</p>
  </body>
</html>
```
When you paste this HTML code into the W3C Validator, it should return no errors because it follows all the rules of valid HTML.
Let us use an errored example and wath it hunt for the error. Paste this HTML code to the W3C Validator;
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Invalid HTML</title>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is missing a closing tag!
    <img src="photo.jpg">
  </body>
</html>
```
We got some errors right? Our `<p>` tag wasn't closed, and our image does not have an `"alt"` attribute. Let's solve the errors and run it again.
Here is the corrected code:
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Valid HTML</title>
  </head>
  <body>
    <h1>Welcome to My Website</h1>
    <p>This is missing a closing tag!</p>
    <img src="photo.jpg" alt="A beautiful photo">
  </body>
</html>
```
## 3. Identifying HTML Errors
**Common HTML Errors**
In most cases, these are the errors you are most likely to make. But that's part of coding, we don't have to get it right the first time. Luckily, W3C corrects us.
* **Missing closing tags**: Every opening tag like `<p>` should have a closing tag like `</p>`.
* **Missing alt attributes for images**: Every `<img>` tag should have an `alt` attribute.
* **Incorrect nesting**: HTML tags should be properly nested. For example, you can’t have `<p><h1>Title</h1></p>` because an `<h1>` tag shouldn’t be inside a `<p>` tag.

## Conclusion
* The **W3C** is an organization that sets the standards for valid HTML.
* **HTML validation** checks if your code follows these standards and helps you find and fix errors.
* You can use the **W3C Validator** to check your HTML code and make sure it’s error-free.
* Common errors include missing closing tags, missing `alt` attributes, and incorrect nesting of tags.

## Resources

* [W3C Validator](https://validator.w3.org/)

## Further Reading
* [Mozilla Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
