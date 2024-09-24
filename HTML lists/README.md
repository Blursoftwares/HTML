# HTML Lists

In this section, we’ll explore **HTML Lists**. A list is like a group of items, just like a grocery list or a list of your favorite toys. There are two main types of lists in HTML: **unordered lists** and **ordered lists**.

---

## Objectives

- **Recognize unordered and ordered HTML lists**: Understand the difference between lists with and without numbers.
- **Create unordered lists**: Learn how to make a list that uses bullets.
- **Identify the ordered list tag**: Find out the tag used to create a numbered list.
- **Create ordered lists**: Learn how to make a list that uses numbers.
- **Nested Lists**: Learn how to make lists inside a list
---

## 1. Unordered vs. Ordered HTML Lists

For this lesson, we are going to be working with our 3 favorite toys; Consider this snippet below;
```html
<body>
  <p>Toy Car</p>
  <p>Doll</p>
</body>
```
The above would add a new line to the page for each toy, but it doesn't exactly indicate how these things are related. However, we may use the built-in `ul`, `ol`, and `li` HTML tags to group relevant list material together. We refer to such a grouping as a "list."

Let's dive right into it!

### **Unordered Lists**:
An unordered list is like a list of items with **bullets** (dots) in front of them. The order doesn't matter, just like when you're writing down your shopping list.

> [!IMPORTANT]
> - **Tag used**: `<ul>`
> - Each item in the list uses the `<li>` tag.

To create an unordered list, use the `<ul>` tag. Inside the list, use the `<li>` tag for each item.

### Example:

```html
<ul>
  <li>Toy car</li>
  <li>Ball</li>
  <li>Doll</li>
</ul>
```
> [!Note]
> This is an unordered list because the items don’t have numbers, just bullets!

### Ordered Lists:
An ordered list is like a numbered list where the items are in a specific order, like steps in a recipe or instructions for a game.

> [!IMPORTANT]
> - **Tag used**: `<ol>`
> - Each item in the list uses the `<li>` tag.

To create an ordered list, use the `<ol> `tag. Inside the list, use the` <li>` tag for each item, just like in an unordered list.
For instance, we can write a routine of what we do once we get home from school:

```html
<ol>
  <li>Brush teeth</li>
  <li>Wash hands</li>
  <li>Go to bed</li>
</ol>
```

> [!Note:]
> This is an ordered list because the items are numbered!

## Nested lists

Sometimes, we might want to put lists **inside** other lists. This is called a **nested list**. You can mix and match both **ordered** and **unordered** lists when you create a nested list, just like grouping toys into boxes and then putting those boxes into bigger boxes.

## 2. Creating a Nested List

You can create a nested list by putting one list (ordered or unordered) **inside** another `<li>` element. Let’s look at how this works.

### Example: Nested Unordered List Inside an Ordered List

```html
<ol>
  <li>Fruits
    <ul>
      <li>Apple</li>
      <li>Banana</li>
    </ul>
  </li>
  <li>Vegetables
    <ul>
      <li>Carrot</li>
      <li>Spinach</li>
    </ul>
  </li>
  <li>Dairy products</li>
     <ul>
      <li>Milk</li>
      <li>Cheese</li>
    </ul>
</ol>
```
> [!Note]
>In this example, the main list is an ordered list (with numbers), and inside some of the items, we have unordered lists (with bullets).

This does not mean that we can't make ordered lists in unordered lists, let us turn things up a little bit more.
```html
<ul>
  <li>Morning Routine
    <ol>
      <li>Brush teeth</li>
      <li>Get dressed</li>
      <li>Eat breakfast</li>
    </ol>
  </li>
  <li>Afternoon Routine
    <ol>
      <li>Have lunch</li>
      <li>Do homework</li>
    </ol>
  </li>
  <li>Evening Routine</li>
</ul>
```
We can make as many list as we need to, just remember to keep things neat and organized! fun right?
Let's try making a list, inside a list, inside a list!

```html
<ol>
  <li>School Subjects
    <ul>
      <li>Math
        <ol>
          <li>Addition</li>
          <li>Subtraction</li>
        </ol>
      </li>
      <li>Science
        <ul>
          <li>Plants</li>
          <li>Animals</li>
        </ul>
      </li>
    </ul>
  </li>
  <li>Sports
<!-- list your favorite sports here -->
</li>
</ol>
```
Copy this code snippet in your editor, and try listing sports and how many players play it for each sport.





