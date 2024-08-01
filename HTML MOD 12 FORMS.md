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
### Module 12: HTML - Forms

HTML forms are used to collect user input and send it to a server for processing. This module covers HTML forms, their attributes, various form elements, input types, input attributes, text areas, buttons, select elements, and labels.

---

#### HTML Forms

- **Description**: HTML forms are used to collect user inputs and send them to a server for processing.
- **Tag**: `<form>`

---

#### HTML Form Attributes

- **`action`**: Specifies the URL where the form data should be sent.
- **`method`**: Specifies the HTTP method to use when sending form data (`GET` or `POST`).
- **`enctype`**: Specifies how the form data should be encoded when sent to the server.
- **`target`**: Specifies where to display the response after submitting the form.
- **`autocomplete`**: Specifies whether the form should have autocomplete on or off.
- **`novalidate`**: Specifies that the form should not be validated when submitted.

**Example**:

```html
<form action="/submit_form" method="post" enctype="multipart/form-data" target="_blank" autocomplete="on" novalidate>
    <!-- Form elements go here -->
</form>
```

---

#### HTML Form Elements

- **`<input>`**: Defines an input field.
- **`<textarea>`**: Defines a multi-line text input.
- **`<button>`**: Defines a clickable button.
- **`<select>`**: Defines a drop-down list.
- **`<option>`**: Defines an option in a drop-down list.
- **`<label>`**: Defines a label for an `<input>` element.

---

#### HTML Input Types

- **`type="text"`**: Defines a single-line text input field.
- **`type="password"`**: Defines a password input field.
- **`type="email"`**: Defines an email input field.
- **`type="number"`**: Defines a numeric input field.
- **`type="date"`**: Defines a date input field.
- **`type="checkbox"`**: Defines a checkbox input field.
- **`type="radio"`**: Defines a radio button input field.
- **`type="submit"`**: Defines a submit button.
- **`type="reset"`**: Defines a reset button.
- **`type="file"`**: Defines a file upload field.

**Example**:

```html
<form action="/submit_form" method="post">
    <input type="text" name="username" placeholder="Enter your username">
    <input type="password" name="password" placeholder="Enter your password">
    <input type="email" name="email" placeholder="Enter your email">
    <input type="number" name="age" min="1" max="100">
    <input type="date" name="birthdate">
    <input type="checkbox" name="subscribe" value="newsletter"> Subscribe to newsletter
    <input type="radio" name="gender" value="male"> Male
    <input type="radio" name="gender" value="female"> Female
    <input type="file" name="profile_picture">
    <input type="submit" value="Submit">
    <input type="reset" value="Reset">
</form>
```

---

#### HTML Input Attributes

- **`value`**: Specifies the default value for the input field.
- **`placeholder`**: Specifies a short hint that describes the expected value of the input field.
- **`name`**: Specifies the name of the input field.
- **`required`**: Specifies that the input field is required.
- **`readonly`**: Specifies that the input field is read-only.
- **`disabled`**: Specifies that the input field is disabled.
- **`maxlength`**: Specifies the maximum number of characters allowed in the input field.
- **`min`** and **`max`**: Specifies the minimum and maximum values for numeric and date inputs.

**Example**:

```html
<form action="/submit_form" method="post">
    <input type="text" name="username" placeholder="Enter your username" required maxlength="20">
    <input type="number" name="age" min="1" max="100" required>
    <input type="submit" value="Submit">
</form>
```

---

#### HTML Input Form Attributes

- **`form`**: Associates the input with a form.
- **`formaction`**: Specifies the URL to send the form data to when the form is submitted.
- **`formenctype`**: Specifies how the form data should be encoded when sent to the server.
- **`formmethod`**: Specifies the HTTP method to use when sending form data.
- **`formtarget`**: Specifies where to display the response after submitting the form.

**Example**:

```html
<form id="myForm" action="/submit_form" method="post">
    <input type="text" name="username" placeholder="Enter your username" required>
    <input type="submit" value="Submit">
</form>

<input type="submit" form="myForm" formaction="/alternative_submit" formmethod="get" formtarget="_blank" value="Submit to alternative URL">
```

---

#### `<textarea>`

- **Description**: Defines a multi-line text input.
- **Attributes**:
  - `cols`: Specifies the visible width of the text area.
  - `rows`: Specifies the visible number of lines in the text area.
  - `maxlength`: Specifies the maximum number of characters allowed in the text area.
  - `placeholder`: Specifies a short hint that describes the expected value of the text area.
  - `required`: Specifies that the text area is required.
  - `readonly`: Specifies that the text area is read-only.
  - `disabled`: Specifies that the text area is disabled.

**Example**:

```html
<form action="/submit_form" method="post">
    <label for="comments">Comments:</label>
    <textarea id="comments" name="comments" cols="30" rows="10" placeholder="Enter your comments here" required maxlength="500"></textarea>
    <input type="submit" value="Submit">
</form>
```

---

#### `<button>`

- **Description**: Defines a clickable button.
- **Attributes**:
  - `type`: Specifies the type of the button (`button`, `submit`, or `reset`).
  - `name`: Specifies the name of the button.
  - `value`: Specifies the initial value of the button.
  - `disabled`: Specifies that the button is disabled.
  - `form`: Associates the button with a form.
  - `formaction`: Specifies the URL to send the form data to when the button is clicked.
  - `formenctype`: Specifies how the form data should be encoded when the button is clicked.
  - `formmethod`: Specifies the HTTP method to use when sending form data when the button is clicked.
  - `formtarget`: Specifies where to display the response after clicking the button.

**Example**:

```html
<form id="myForm" action="/submit_form" method="post">
    <input type="text" name="username" placeholder="Enter your username" required>
    <button type="submit" formaction="/alternative_submit" formmethod="get" formtarget="_blank">Submit to alternative URL</button>
    <button type="reset">Reset</button>
</form>
```

---

#### `<select>`

- **Description**: Defines a drop-down list.
- **Attributes**:
  - `name`: Specifies the name of the drop-down list.
  - `multiple`: Specifies that multiple options can be selected.
  - `required`: Specifies that the drop-down list is required.
  - `disabled`: Specifies that the drop-down list is disabled.
  - `form`: Associates the drop-down list with a form.

**Example**:

```html
<form action="/submit_form" method="post">
    <label for="cars">Choose a car:</label>
    <select id="cars" name="cars" required>
        <option value="volvo">Volvo</option>
        <option value="saab">Saab</option>
        <option value="mercedes">Mercedes</option>
        <option value="audi">Audi</option>
    </select>
    <input type="submit" value="Submit">
</form>
```

---

#### `<label>`

- **Description**: Defines a label for an `<input>` element.
- **Attributes**:
  - `for`: Specifies which form element a label is bound to.

**Example**:

```html
<form action="/submit_form" method="post">
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" required>
    <input type="submit" value="Submit">
</form>
```

---

### Interview Questions

1. **What is the purpose of the `<form>` element in HTML?**
   - **Answer**: The `<form>` element is used to collect user inputs and send them to a server for processing.

2. **List and explain the attributes of the `<form>` element.**
   - **Answer**:
     - `action`: Specifies the URL where the form data should be sent.
     - `method`: Specifies the HTTP method to use when sending form data (`GET` or `POST`).
     - `enctype`: Specifies how the form data should be encoded when sent to the server.
     - `target`: Specifies where to display the response after submitting the form.
     - `

autocomplete`: Specifies whether the form should have autocomplete on or off.
     - `novalidate`: Specifies that the form should not be validated when submitted.

3. **Provide examples of different HTML input types and their attributes.**
   - **Answer**:
     ```html
     <input type="text" name="username" placeholder="Enter your username" required maxlength="20">
     <input type="password" name="password" placeholder="Enter your password" required>
     <input type="email" name="email" placeholder="Enter your email" required>
     <input type="number" name="age" min="1" max="100" required>
     <input type="date" name="birthdate" required>
     <input type="checkbox" name="subscribe" value="newsletter"> Subscribe to newsletter
     <input type="radio" name="gender" value="male"> Male
     <input type="radio" name="gender" value="female"> Female
     <input type="file" name="profile_picture" required>
     <input type="submit" value="Submit">
     <input type="reset" value="Reset">
     ```

4. **Explain how to use the `<textarea>` element and its attributes.**
   - **Answer**: 
     ```html
     <textarea id="comments" name="comments" cols="30" rows="10" placeholder="Enter your comments here" required maxlength="500"></textarea>
     ```

5. **How do you associate a `<label>` element with an `<input>` element?**
   - **Answer**: You associate a `<label>` element with an `<input>` element using the `for` attribute. The value of the `for` attribute should match the `id` of the `<input>` element.
     ```html
     <label for="username">Username:</label>
     <input type="text" id="username" name="username" required>
     ```

These questions and examples should help solidify your understanding of HTML forms and their elements.