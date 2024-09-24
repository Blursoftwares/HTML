# HTML Tables

## Objectives
- **Recognize basic HTML table elements**: Learn the parts that make up a table, like rows and columns.
- **Create HTML tables**: Discover how to create your own table in HTML.

## Introduction

Tables in HTML help us organize information in **rows** and **columns**, just like the tables you see in books or worksheets! In this section, we’ll learn how to create a basic table and understand the different parts of a table.

## 1. What is a Table?

A **table** is like a grid made up of **rows** (horizontal lines) and **columns** (vertical lines) that organize information. Tables can be used to show things like schedules, scores, or data.

### Basic Table Structure:

- **`<table>`**: This tag creates the table.
- **`<tr>`**: This stands for “table row” and is used to make rows (horizontal lines).
- **`<td>`**: This stands for “table data” and is used to make columns (vertical lines) inside the rows.

---

## 2. Recognizing Basic HTML Table Elements

There are a few key elements that make up a table:

- **`<table>`**: The container that holds the entire table.
- **`<tr>`** (Table Row): This creates a row in the table.
- **`<td>`** (Table Data): This creates a cell or column within a row.
- **`<th>`** (Table Header): This is used to create a header cell, usually bold, to label the top of a column.

---

## 3. Creating a Basic HTML Table

Let’s start by creating a simple table with **two rows** and **two columns**. This table list's Alice and Bob's ages respectively


```html
<table>
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>5</td>
  </tr>
  <tr>
    <td>Bob</td>
    <td>6</td>
  </tr>
</table>
```

In this example:

* The first row (<tr>) is a header row, and we use <th> to make the text bold.
* The second and third rows contain data using <td>.

## 4. Adding More Rows and Columns
You can easily add more rows and columns by adding more `<tr>` and `<td>` elements.

Let's create a table for James, a top performing student in the school.

```html
<table>
  <tr>
    <th>Subject</th>
    <th>Score</th>
  </tr>
  <tr>
    <td>Math</td>
    <td>95</td>
  </tr>
  <tr>
    <td>Science</td>
    <td>89</td>
  </tr>
  <tr>
    <td>History</td>
    <td>92</td>
  </tr>
</table>
```

In this table, we added more rows to show three different subjects and their corresponding scores.

## 5. Spanning Columns or Rows

Sometimes, we want a cell to span multiple columns or rows. This is done using the `colspan` and `rowspan` attributes.

### Example:
```html
<table>
  <tr>
    <th colspan="2">Name and Age</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>5</td>
  </tr>
</table>
```

## Conclusion
* Tables in HTML are created with the `<table>` tag.
* Rows are created with `<tr>`, and columns are created with `<td>`.
* Headers (bold labels) use the `<th>` tag.
* You can span multiple columns or rows using the `colspan` and `rowspan` attributes.
