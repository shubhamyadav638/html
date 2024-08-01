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
# Module 3: HTML Headers

## Title
- **Definition**: The `<title>` tag defines the title of the document, shown in the browser's title bar or tab.
- **Example**:
    ```html
    <head>
        <title>My Web Page</title>
    </head>
    ```

## Base
- **Definition**: The `<base>` tag specifies the base URL for all relative URLs in a document. Only one `<base>` element is allowed in a document.
- **Example**:
    ```html
    <head>
        <base href="https://www.example.com/" target="_blank">
    </head>
    ```

## Link
- **Definition**: The `<link>` tag defines a relationship between the current document and an external resource. It's commonly used to link to stylesheets.
- **Example**:
    ```html
    <head>
        <link rel="stylesheet" href="styles.css">
    </head>
    ```

## Styles
- **Definition**: The `<style>` tag is used to define internal CSS styles within an HTML document.
- **Example**:
    ```html
    <head>
        <style>
            body {
                background-color: lightblue;
            }
            h1 {
                color: navy;
            }
        </style>
    </head>
    ```

## Script
- **Definition**: The `<script>` tag is used to embed or reference executable code; this is typically used to include JavaScript.
- **Example**:
    ```html
    <head>
        <script>
            function sayHello() {
                alert('Hello, World!');
            }
        </script>
    </head>
    ```

## Meta
- **Definition**: The `<meta>` tag provides metadata about the HTML document. Metadata is not displayed on the page but is machine-parsable.
- **Common Uses**:
  - **Character Set**: 
      ```html
      <meta charset="UTF-8">
      ```
  - **Viewport**:
      ```html
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      ```
  - **Description**:
      ```html
      <meta name="description" content="Free Web tutorials">
      ```
  - **Keywords**:
      ```html
      <meta name="keywords" content="HTML, CSS, JavaScript">
      ```
  - **Author**:
      ```html
      <meta name="author" content="John Doe">
      ```

## Interview Questions

### Title
1. **What is the purpose of the `<title>` tag in HTML?**
   - The `<title>` tag defines the title of the document, which is displayed in the browser's title bar or tab.
   
2. **Can multiple `<title>` tags be used in a single HTML document?**
   - No, only one `<title>` tag is allowed in a single HTML document.

### Base
1. **What is the function of the `<base>` tag in HTML?**
   - The `<base>` tag specifies the base URL for all relative URLs in a document.

2. **How many `<base>` tags can be used in a single HTML document?**
   - Only one `<base>` element is allowed in a document.

### Link
1. **What is the `<link>` tag used for in HTML?**
   - The `<link>` tag is used to define a relationship between the current document and an external resource, commonly for linking to stylesheets.

2. **What attribute of the `<link>` tag specifies the location of the stylesheet?**
   - The `href` attribute specifies the location of the stylesheet.

### Styles
1. **What is the purpose of the `<style>` tag in HTML?**
   - The `<style>` tag is used to define internal CSS styles within an HTML document.

2. **Can CSS be included both internally and externally in an HTML document?**
   - Yes, CSS can be included both internally using the `<style>` tag and externally using the `<link>` tag.

### Script
1. **What does the `<script>` tag do in an HTML document?**
   - The `<script>` tag is used to embed or reference executable code, typically JavaScript.

2. **Can JavaScript code be included directly within an HTML document?**
   - Yes, JavaScript code can be included directly within an HTML document using the `<script>` tag.

### Meta
1. **What is the purpose of the `<meta>` tag in HTML?**
   - The `<meta>` tag provides metadata about the HTML document, such as character set, viewport settings, and descriptions.

2. **Can multiple `<meta>` tags be used in an HTML document?**
   - Yes, multiple `<meta>` tags can be used to provide different pieces of metadata.

This overview of HTML headers introduces you to the key elements used in the `<head>` section of an HTML document, providing a foundation for understanding how to include metadata, styles, scripts, and more.
