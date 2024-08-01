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

### Module 11: HTML - `<iframe>`

An `<iframe>` (inline frame) is used to embed another document within the current HTML document. Here are the detailed notes on using `<iframe>` as well as its attributes and use cases.

---

#### `<iframe>`

- **Description**: The `<iframe>` element is used to embed another HTML document within the current document.
- **Attributes**:
  - `src`: Specifies the URL of the document to embed.
  - `width`: Specifies the width of the iframe.
  - `height`: Specifies the height of the iframe.
  - `name`: Specifies the name of the iframe.
  - `sandbox`: Enables an extra set of restrictions for the content in the iframe.
  - `allow`: Specifies a feature policy for the iframe.
  - `allowfullscreen`: Allows the iframe to be displayed in full-screen mode.
  - `loading`: Specifies whether the iframe should be loaded lazily.
  - `referrerpolicy`: Specifies the referrer policy for the iframe.
  - `srcdoc`: Specifies the HTML content to display in the iframe.
  - `frameborder`: Specifies whether or not to display a border around the iframe.
  - `scrolling`: Specifies whether or not to display scrollbars in the iframe.

**Use Case**: Embedding external content or another web page within the current page.

---

### Example

#### Basic `<iframe>` Example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML IFrame Example</title>
</head>
<body>
    <h1>Embedding an External Web Page</h1>
    <iframe src="https://www.example.com" width="600" height="400" name="exampleIframe" frameborder="1" scrolling="yes" allowfullscreen></iframe>
</body>
</html>
```

#### Explanation of Attributes:
- **`src`**: URL of the page to be embedded.
- **`width`**: Width of the iframe in pixels or percentage.
- **`height`**: Height of the iframe in pixels or percentage.
- **`name`**: Name of the iframe, used as a target for links.
- **`frameborder`**: Specifies whether to display a border around the iframe (0 or 1).
- **`scrolling`**: Specifies whether to allow scrolling within the iframe (`yes`, `no`, `auto`).
- **`allowfullscreen`**: Enables full-screen mode for the iframe content.

---

### Using `<iframe>` as the Target

You can use an iframe as the target for links and form submissions. By setting the `target` attribute of a link or a form to the name of the iframe, the linked page or form results will be displayed in the iframe.

#### Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IFrame as Target Example</title>
</head>
<body>
    <h1>IFrame as Target</h1>
    
    <!-- Links that target the iframe -->
    <p>
        <a href="https://www.example.com" target="myIframe">Go to Example.com</a> |
        <a href="https://www.wikipedia.org" target="myIframe">Go to Wikipedia</a>
    </p>
    
    <!-- Form that targets the iframe -->
    <form action="https://www.example.com/search" target="myIframe">
        <label for="search">Search Example.com:</label>
        <input type="text" id="search" name="q">
        <input type="submit" value="Search">
    </form>
    
    <!-- IFrame -->
    <iframe src="about:blank" width="600" height="400" name="myIframe" frameborder="1" scrolling="yes" allowfullscreen></iframe>
</body>
</html>
```

#### Explanation:
- **Links**: The `target="myIframe"` attribute makes the linked pages open within the iframe named "myIframe".
- **Form**: The `target="myIframe"` attribute makes the form submission results open within the iframe named "myIframe".
- **IFrame**: The `name="myIframe"` attribute assigns a name to the iframe, making it a target for links and forms.

---

### Interview Questions

1. **What is the purpose of the `<iframe>` element in HTML?**
   - **Answer**: The `<iframe>` element is used to embed another HTML document within the current document.

2. **How can you use an `<iframe>` as a target for links and form submissions?**
   - **Answer**: By setting the `target` attribute of a link or a form to the name of the iframe, the linked page or form results will be displayed in the iframe.

3. **List and explain the attributes of the `<iframe>` element.**
   - **Answer**: 
     - `src`: URL of the document to embed.
     - `width`: Width of the iframe.
     - `height`: Height of the iframe.
     - `name`: Name of the iframe, used as a target.
     - `sandbox`: Enables extra restrictions.
     - `allow`: Specifies a feature policy.
     - `allowfullscreen`: Allows full-screen mode.
     - `loading`: Specifies lazy loading.
     - `referrerpolicy`: Sets the referrer policy.
     - `srcdoc`: HTML content to display.
     - `frameborder`: Border around the iframe.
     - `scrolling`: Scrollbars in the iframe.

4. **Provide an example of using an `<iframe>` to display content from another website.**
   - **Answer**: 
     ```html
     <iframe src="https://www.example.com" width="600" height="400" name="exampleIframe" frameborder="1" scrolling="yes" allowfullscreen></iframe>
     ```

5. **Demonstrate how to use an `<iframe>` as a target for a link.**
   - **Answer**: 
     ```html
     <a href="https://www.example.com" target="myIframe">Go to Example.com</a>
     <iframe name="myIframe" width="600" height="400"></iframe>
     ```

These questions and examples should help solidify your understanding of `<iframe>` and its usage in HTML.
