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
## Module 5: HTML - Grouping Using DIV and SPAN

### Div Tag
The `<div>` tag is used to group block-level content. It is a block-level element that is commonly used to structure the layout of web pages.

#### Common Uses
- Grouping content for styling purposes using CSS.
- Creating layout sections such as headers, footers, and sidebars.
- Wrapping multiple elements for applying JavaScript functionality.

#### Example
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        .container {
            width: 80%;
            margin: 0 auto;
            border: 1px solid #ccc;
            padding: 10px;
        }
        .header, .footer {
            background-color: #f1f1f1;
            padding: 10px;
        }
        .content {
            padding: 10px;
        }
    </style>
    <title>Div Example</title>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Header Section</h1>
        </div>
        <div class="content">
            <p>This is the content section.</p>
        </div>
        <div class="footer">
            <p>Footer Section</p>
        </div>
    </div>
</body>
</html>
```

### Span Tag
The `<span>` tag is an inline container used to mark up a part of a text or a document. It is an inline element that is used for grouping inline elements for styling purposes.

#### Common Uses
- Styling a part of the text with CSS.
- Applying JavaScript functionality to a part of the text.
- Wrapping text or other inline elements without disrupting the document flow.

#### Example
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        .highlight {
            background-color: yellow;
        }
        .bold {
            font-weight: bold;
        }
    </style>
    <title>Span Example</title>
</head>
<body>
    <p>This is a normal paragraph.</p>
    <p>This is a <span class="highlight">highlighted text</span> in a paragraph.</p>
    <p>This is a <span class="bold">bold text</span> in a paragraph.</p>
</body>
</html>
```

## Interview Questions and Answers

1. **What is the purpose of the `<div>` tag in HTML?**
   - **Answer:** The `<div>` tag is used to group block-level content and is commonly used to structure the layout of web pages. It helps in organizing and styling sections of the content.

2. **How is the `<span>` tag different from the `<div>` tag?**
   - **Answer:** The `<span>` tag is an inline element used to group inline content, whereas the `<div>` tag is a block-level element used to group block-level content. The `<span>` tag does not disrupt the document flow, while the `<div>` tag creates a new block.

3. **How can you use the `<div>` tag to create a layout section?**
   - **Answer:** You can use the `<div>` tag to wrap different sections of the layout, such as headers, footers, and sidebars. By applying CSS styles to these `<div>` elements, you can control their appearance and layout.
   - **Code Example:**
     ```html
     <div class="header">Header Section</div>
     <div class="content">Content Section</div>
     <div class="footer">Footer Section</div>
     ```

4. **Give an example of how to use the `<span>` tag to style a part of a text.**
   - **Answer:** You can use the `<span>` tag to wrap a part of the text and apply CSS styles to it.
   - **Code Example:**
     ```html
     <p>This is a <span class="highlight">highlighted text</span> in a paragraph.</p>
     <style>
         .highlight {
             background-color: yellow;
         }
     </style>
     ```

5. **Can you nest `<div>` and `<span>` tags? Provide an example.**
   - **Answer:** Yes, you can nest `<div>` and `<span>` tags within each other.
   - **Code Example:**
     ```html
     <div class="container">
         <div class="header">
             <h1>Header <span class="highlight">Section</span></h1>
         </div>
         <div class="content">
             <p>This is the <span class="bold">content</span> section.</p>
         </div>
         <div class="footer">
             <p>Footer <span class="highlight">Section</span></p>
         </div>
     </div>
     <style>
         .highlight {
             background-color: yellow;
         }
         .bold {
             font-weight: bold;
         }
     </style>
     ```

These notes, interview questions, and code examples provide a comprehensive overview of grouping using the `<div>` and `<span>` tags in HTML.