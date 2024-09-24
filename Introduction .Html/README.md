# HTML - Beginner syllabus
# Introduction to HTML
**What is HTML**

HTML is the skeleton of every webpage ,it provides the structure to content appearing on your page such as images , texts , videos etc

## What does HTML stand for ##
__Hypertext markup Language__
### A markup language ##
> is a computer language that defines the structure and presentation of raw text
> In HTML the computer can interpret raw text that is wrapped in HTML Elements
> Hyper text is text displayed on computer or device that provides access to other text through links also know as **Hyperlinks**

# HTML Anatomy
 **Week 1**

HTML is composed of Elements
>[!NOTE]
these elements structure the webpage and defines its content
![](https://curriculum-content.s3.amazonaws.com/html-basics/welcome-to-html/Image_48_HTMLBannerGraphic.png)                        

in every html document has specific required tags , Because they are required every time we create a webpage.

## Basic HTML Document Structure
**A DOCTYPE tag** 
<!DOCTYPE html>
at the top of every HTML document you have to start with the same element DOCTYPE
it 

the DOCTYPE element as with all HTML starts with a < and ends with a > uniquely the DOCTYPE starts with an exclamation point ! , followed by DOCTYPE then we specify which html we want to use . INn HTML5 we just write html and the browswer will interpret in as HTML 5
its display is <!DOCTYPE html>

**HTML**
the next element is required <html>this tells the browser that anything in between the html opening and closing tags is to be read as HTML CODE
one important attribute to include in <html>tag is Lang which describes which language the webpage is written in in our case we use ENGLISH lang="en". it helps the google engine to know what language a page is written in

          <html lang="en"></html>

**The Head section and its content**
inside our html tags we divide the page into 2 __head__  and __Body__ which both play unique roles
the head is not visible to our website visitor, but contains alot of useful information about our page
in our head section we place a number of specific tags
<links>
<title>

**Links**
the <link>tag is for importing files



**Title**
the<title> is where the title of your webpage goes in , text added inside the title tag will appear on the browser tab
<title>Story about my school</title>
unlike the link tag the title tag has an opening and closing tag

the head section we are able to add relevant data about our webpage as a whole.

## The Body 
one key HTML elements we use to build webpages is the body element
>[!NOTE]
>only content inside the opening and closing body tag will be displayed on the screen
```HTML
<body>
what will be displayed on the screen
</body>
```

once your html has body many different things can be included to be displayed things like;

1 *image*
2 *videos*
3 *paragraphs* etc.

```html
<body>
  <p> I love kenya</p>
</body> 
```
### The HTML tags

There is only 6 heading tags 
The <p> tag is used tag is used to describe  paragraphs
<h1> to <h6> are used to define html headings
<h1> defines the most important heading.
<h6> defines the least important heading.

```html
<p>Today it's a sunny day, and you're enjoying a big scoop of your favorite ice cream. It's sweet, and creamy What’s your favorite flavor?</p>
```

### Hierarchy

HTML is organised as a collection of family tree relationship,
when an element is contained or added inside another element it is said to be a child of that element.
the child element is said to be nested inside the parent element

```html
<body>
  <p>I LOVE KENYA</p>
</body>
```
the example above the p tag is nested inside the body tag the p element is said to be a child of the body element and the body is considered to be the parent . you add spaces of indentation to create the relationship,
since they can be different levels of nesting the relationship between parent and children is know as hierarchy
understanding hierarchy is important because child element can inherit behaviour and styling from their parent element
