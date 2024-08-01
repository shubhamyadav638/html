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
# Module 8: HTML Images

## 1. Image
Images are an essential part of web pages, used to enhance visual appeal and convey information.

### Syntax:
```html
<img src="url" alt="description" />
```

### Attributes:
- `src`: Specifies the path to the image.
- `alt`: Provides alternative text for the image if it cannot be displayed.
- `width` and `height`: Define the dimensions of the image.
- `title`: Provides additional information about the image, often displayed as a tooltip.

### Example:
```html
<img src="https://www.example.com/image.jpg" alt="Example Image" width="300" height="200" />
```

### Key Points:
- The `<img>` tag is used to embed images in HTML.
- Always include the `alt` attribute for accessibility and SEO.

## 2. Image Mapping
Image mapping allows you to define clickable areas on an image, linking different parts of the image to different destinations.

### Syntax:
```html
<img src="image.jpg" alt="Image Map" usemap="#mapname" />
<map name="mapname">
  <area shape="rect" coords="34,44,270,350" href="https://www.example1.com" alt="Link 1" />
  <area shape="circle" coords="337,300,44" href="https://www.example2.com" alt="Link 2" />
  <area shape="poly" coords="362,116,369,192,456,196,453,122" href="https://www.example3.com" alt="Link 3" />
</map>
```

### Attributes:
- `usemap`: Associates the image with a `<map>` element.
- `<map>`: Defines the image map.
- `<area>`: Defines the clickable areas within the image map.

### Shapes:
- `rect`: Rectangle (defined by top-left and bottom-right coordinates).
- `circle`: Circle (defined by center coordinates and radius).
- `poly`: Polygon (defined by a series of coordinates).

### Example:
```html
<img src="worldmap.jpg" alt="World Map" usemap="#worldmap" />
<map name="worldmap">
  <area shape="rect" coords="0,0,82,126" href="https://www.example1.com" alt="North America" />
  <area shape="circle" coords="90,58,3" href="https://www.example2.com" alt="Greenland" />
  <area shape="poly" coords="100,100,120,140,140,100,100,100" href="https://www.example3.com" alt="Triangle" />
</map>
```

### Key Points:
- Image maps create interactive areas within an image.
- Use the `<map>` and `<area>` tags to define the map and its clickable regions.

## 3. Background Images
Background images are used to add visual interest to the background of an element.

### Syntax:
```html
<style>
  element {
    background-image: url('image.jpg');
  }
</style>
```

### CSS Properties:
- `background-image`: Specifies the background image.
- `background-repeat`: Controls how the background image repeats (e.g., `no-repeat`, `repeat-x`, `repeat-y`).
- `background-position`: Sets the initial position of the background image.
- `background-size`: Specifies the size of the background image (e.g., `cover`, `contain`).

### Example:
```html
<style>
  body {
    background-image: url('background.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
  }
</style>
```

### Key Points:
- Use CSS to add and style background images.
- Control the repetition, position, and size of background images using CSS properties.

## Interview Questions and Answers

### Q1: How do you embed an image in an HTML document?
**A1:** You can embed an image using the `<img>` tag and specifying the `src` attribute for the image source. For example:
```html
<img src="image.jpg" alt="Description" />
```

### Q2: What is the purpose of the `alt` attribute in the `<img>` tag?
**A2:** The `alt` attribute provides alternative text for the image, which is displayed if the image cannot be loaded. It also improves accessibility and SEO.

### Q3: How do you create an image map in HTML?
**A3:** You create an image map by using the `<map>` tag to define the map and the `<area>` tag to define clickable areas. The `usemap` attribute on the `<img>` tag associates the image with the map. For example:
```html
<img src="image.jpg" alt="Image Map" usemap="#mapname" />
<map name="mapname">
  <area shape="rect" coords="34,44,270,350" href="https://www.example.com" alt="Link" />
</map>
```

### Q4: What are the different shapes you can define in an image map?
**A4:** You can define the following shapes in an image map:
- `rect`: Rectangle, defined by top-left and bottom-right coordinates.
- `circle`: Circle, defined by center coordinates and radius.
- `poly`: Polygon, defined by a series of coordinates.

### Q5: How do you add a background image to an element using CSS?
**A5:** You can add a background image using the `background-image` property in CSS. For example:
```css
element {
  background-image: url('image.jpg');
}
```

### Q6: How can you control the repetition of a background image in CSS?
**A6:** You can control the repetition using the `background-repeat` property. Possible values include `no-repeat`, `repeat`, `repeat-x`, and `repeat-y`. For example:
```css
element {
  background-image: url('image.jpg');
  background-repeat: no-repeat;
}
```

### Q7: What is the `background-size` property used for?
**A7:** The `background-size` property specifies the size of the background image. Values include `cover`, `contain`, and specific dimensions (e.g., `100px 200px`). For example:
```css
element {
  background-image: url('image.jpg');
  background-size: cover;
}
```

### Q8: How can you center a background image using CSS?
**A8:** You can center a background image using the `background-position` property with the value `center`. For example:
```css
element {
  background-image: url('image.jpg');
  background-position: center;
}
```
```