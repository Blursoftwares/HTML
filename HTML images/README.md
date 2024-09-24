# HTML Images

## Objectives
- **Recognize the `img` tag**: Learn about the special tag used to add images in HTML.
- **Use `img` tag attributes**: Understand how to make images look just the way you want using attributes like `src`, `alt`, `width`, and `height`.
- **Create images**: Discover how to add your own images to a webpage.

## Introduction
Images are important for creating visually appealing and engaging websites. Can you imagine the internet without them? No Youtube. There are no movies! No Tiktok all. The internet would be a quite boring and depressing place right?

## 1. Recognize the `img` Tag

The **`<img>` tag** is used to display an image on a webpage. Unlike other tags like `<p>` or `<h1>`, the `<img>` tag doesn’t have a closing tag because it’s a **self-closing** tag.

### Example:

```html
<img src="toy.jpg" alt="A toy car">
```

In this example:
* The `src` attribute tells the browser where to find the image (its source).
* The `alt` attribute describes the image for users who can’t see it or for browsers that can’t load the image.

Sometimes we need tto specify the image size. We can do this by specifying the width and height of the image. Take a look at the example below

```html
<img src="https://i.natgeofe.com/n/548467d8-c5f1-4551-9f58-6817a8d2c45e/NationalGeographic_2572187_square.jpg" alt="A cute cat" width="300" height="200">
```

This would display a 300x200 pixel image of a cute cat. If the image doesn't load, the text "A cute cat" will be shown instead.

## 3. Creating Images
First, you need to have an image saved either on your computer or find one online. If it’s online, you can use the image’s URL.

> [!Tip]
> A URL is the path to the image, it looks like this: "https://www.example.com/bird.jpg"

Once you have the image, use the <img> tag and set the src attribute to point to your image file or URL. If your image is in your local computer, you can
write it as:
```html
<img src="images/dog.jpg" alt="A happy dog" width="400">
```
In this example, we’re pointing to an image called "dog.jpg" saved in the images folder. Quick question, what does the `width` attribute do?

Alternatively, if you are using an image from the internet, you can structure your code like this:
```html
<img src="https://www.example.com/bird.jpg" alt="A bird flying" width="350">
```

## 4. Responsive Images
Sometimes, we want images to automatically adjust based on the size of the device. You can use the CSS property `max-width` to make images responsive. Don't worry too much
about this, we'll talk more about it later on.
```html
<img src="butterfly.png" alt="A colorful butterfly" style="max-width: 100%;">
```

## Conclusion
* The `<img>` tag is used to add images to a webpage.
* Use the `src` attribute to specify the image source and `alt` to describe the image.
* You can control the size of your image with the `width` and `height` attributes.

Woohoo! we can now add pictures to our website and make our pages more visually appealing!





