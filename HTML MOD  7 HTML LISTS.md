<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Module 4</title>
    <style>
        body {
            background-color: black;
            color: white;
        }
        h1, h2, h3, h4, h5, h6 {
            color: white;
        }
    </style>
</head>
<body>
```markdown
# Module 7: HTML Lists

## 1. Unordered Lists
Unordered lists are used to group a set of related items in no particular order. They are typically rendered as bulleted lists.

### Syntax:
```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

### Example:
```html
<ul>
  <li>Apples</li>
  <li>Oranges</li>
  <li>Bananas</li>
</ul>
```

### Key Points:
- The `<ul>` tag defines the unordered list.
- The `<li>` tag defines each list item.
- The items are usually rendered with bullet points.

## 2. Ordered Lists
Ordered lists are used to group a set of related items in a specific order. They are typically rendered as numbered lists.

### Syntax:
```html
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>
```

### Example:
```html
<ol>
  <li>Step 1</li>
  <li>Step 2</li>
  <li>Step 3</li>
</ol>
```

### Key Points:
- The `<ol>` tag defines the ordered list.
- The `<li>` tag defines each list item.
- The items are usually rendered with numbers.

## 3. Definition Lists
Definition lists are used to group terms and their definitions. They are typically rendered with terms and descriptions.

### Syntax:
```html
<dl>
  <dt>Term 1</dt>
  <dd>Description of Term 1</dd>
  <dt>Term 2</dt>
  <dd>Description of Term 2</dd>
</dl>
```

### Example:
```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>
```

### Key Points:
- The `<dl>` tag defines the definition list.
- The `<dt>` tag defines the term.
- The `<dd>` tag defines the description of the term.

## Interview Questions and Answers

### Q1: What is an unordered list?
**A1:** An unordered list is used to group a set of related items in no particular order. It is created using the `<ul>` tag, with each item in the list wrapped in an `<li>` tag.

### Q2: How do you create an ordered list in HTML?
**A2:** An ordered list is created using the `<ol>` tag, with each item in the list wrapped in an `<li>` tag. The items are typically rendered with numbers.

### Q3: What is the difference between an unordered list and an ordered list?
**A3:** An unordered list (`<ul>`) displays items in no particular order, typically with bullet points. An ordered list (`<ol>`) displays items in a specific order, typically with numbers.

### Q4: How do you create a definition list in HTML?
**A4:** A definition list is created using the `<dl>` tag. Each term is defined with the `<dt>` tag, and each description is defined with the `<dd>` tag.

### Q5: Can you nest lists in HTML? If so, how?
**A5:** Yes, you can nest lists in HTML. To nest a list, place a `<ul>` or `<ol>` element inside an `<li>` element of another list. For example:
```html
<ul>
  <li>Item 1
    <ul>
      <li>Subitem 1</li>
      <li>Subitem 2</li>
    </ul>
  </li>
  <li>Item 2</li>
</ul>
```
```