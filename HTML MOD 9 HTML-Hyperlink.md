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
## Module 9: HTML-Hyperlink

### Anchor Tag
The anchor tag `<a>` is used to create hyperlinks, which are essential for navigating between different pages on the web. The `href` attribute specifies the URL of the page the link goes to.

#### Example
```html
<!DOCTYPE html>
<html>
<head>
    <title>Anchor Tag Example</title>
</head>
<body>
    <h1>Example of an Anchor Tag</h1>
    <p>Visit the <a href="https://www.example.com">Example Website</a> for more information.</p>
</body>
</html>
```

### URL - Uniform Resource Locator
A URL (Uniform Resource Locator) is the address of a resource on the web. It consists of several parts:
- **Scheme**: Specifies the protocol (e.g., http, https, ftp).
- **Host**: Domain name or IP address of the server.
- **Path**: Specific resource within the host.
- **Query String**: Optional, provides additional parameters.

#### Example
html
<!DOCTYPE html>
<html>
<head>
    <title>URL Example</title>
</head>
<body>
    <h1>URL Structure</h1>
    <p>Scheme: <code>https</code></p>
    <p>Host: <code>www.example.com</code></p>
    <p>Path: <code>/path/to/resource</code></p>
    <p>Query String: <code>?key1=value1&key2=value2</code></p>
</body>
</html>


### Relative Address
A relative address provides the path to a resource relative to the current page's location. It is useful for linking to resources within the same website.

#### Example
```html
<!DOCTYPE html>
<html>
<head>
    <title>Relative Address Example</title>
</head>
<body>
    <h1>Relative Address</h1>
    <p>Go to the <a href="about.html">About Page</a>.</p>
</body>
</html>
```

### Absolute Address
An absolute address provides the complete URL of a resource, including the scheme, host, and path. It is used to link to resources outside the current website.

#### Example
```html
<!DOCTYPE html>
<html>
<head>
    <title>Absolute Address Example</title>
</head>
<body>
    <h1>Absolute Address</h1>
    <p>Visit the <a href="https://www.example.com/about.html">Example Website's About Page</a>.</p>
</body>
</html>
```

## Interview Questions and Answers

1. **What is the purpose of the anchor (`<a>`) tag in HTML?**
   - **Answer:** The anchor tag `<a>` is used to create hyperlinks, allowing users to navigate between different pages or resources on the web. The `href` attribute specifies the URL of the target page or resource.

2. **What are the components of a URL?**
   - **Answer:** A URL consists of several components: the scheme (protocol), host (domain name or IP address), path (specific resource within the host), and an optional query string (additional parameters).

3. **Explain the difference between a relative and an absolute address.**
   - **Answer:** A relative address provides the path to a resource relative to the current page's location and is used for internal links within the same website. An absolute address provides the complete URL of a resource, including the scheme, host, and path, and is used to link to external resources.

4. **When would you use a relative address instead of an absolute address?**
   - **Answer:** A relative address is used when linking to resources within the same website, as it is shorter and easier to manage if the domain changes. An absolute address is used when linking to resources outside the current website.

5. **What is the purpose of the `href` attribute in the anchor tag?**
   - **Answer:** The `href` attribute in the anchor tag specifies the URL of the page or resource the link goes to. It defines the destination of the hyperlink.

These notes, interview questions, and code examples provide a comprehensive overview of handling hyperlinks in HTML, including the use of anchor tags, understanding URLs, and distinguishing between relative and absolute addresses.