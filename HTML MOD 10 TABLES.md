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


### Module 10: HTML - Table

HTML tables are used to display data in a tabular format. Here are the detailed notes on various HTML table elements and their attributes:

---

#### `<table>`

- **Description**: The `<table>` element defines a table in HTML.
- **Attributes**:
  - `border`: Specifies the width of the border around the table.
  - `cellpadding`: Specifies the space between the cell wall and the cell content.
  - `cellspacing`: Specifies the space between cells.
  - `width`: Specifies the width of the table.
  - `height`: Specifies the height of the table.
  - `align`: Specifies the alignment of the table (left, center, right).
  - `bgcolor`: Specifies the background color of the table.

**Use Case**: Creating the basic structure of a table.

---

#### `<th>`

- **Description**: The `<th>` element defines a header cell in a table.
- **Attributes**:
  - `abbr`: Specifies an abbreviated version of the header cell content.
  - `scope`: Specifies the scope of the header cell (col, colgroup, row, rowgroup).
  - `colspan`: Specifies the number of columns a header cell should span.
  - `rowspan`: Specifies the number of rows a header cell should span.
  - `headers`: Specifies one or more header cells a cell is related to.
  
**Use Case**: Defining header cells to display titles or labels for table columns or rows.

---

#### `<tr>`

- **Description**: The `<tr>` element defines a row in a table.
- **Attributes**:
  - `align`: Specifies the alignment of the content in the row (left, center, right, justify).
  - `bgcolor`: Specifies the background color of the row.
  - `valign`: Specifies the vertical alignment of the content in the row (top, middle, bottom, baseline).
  
**Use Case**: Creating a row to group cells within a table.

---

#### `<td>`

- **Description**: The `<td>` element defines a standard data cell in a table.
- **Attributes**:
  - `colspan`: Specifies the number of columns a cell should span.
  - `rowspan`: Specifies the number of rows a cell should span.
  - `headers`: Specifies one or more header cells a cell is related to.
  - `align`: Specifies the alignment of the content in the cell (left, center, right, justify).
  - `bgcolor`: Specifies the background color of the cell.
  - `valign`: Specifies the vertical alignment of the content in the cell (top, middle, bottom, baseline).
  
**Use Case**: Adding data to individual cells within a row.

---

#### `<caption>`

- **Description**: The `<caption>` element defines a table caption.
- **Attributes**:
  - `align`: Specifies the alignment of the caption (top, bottom, left, right).
  
**Use Case**: Providing a title or explanation for the table.

---

#### `<thead>`

- **Description**: The `<thead>` element groups the header content in a table.
- **Attributes**:
  - `align`: Specifies the alignment of the content in the header (left, center, right, justify).
  - `valign`: Specifies the vertical alignment of the content in the header (top, middle, bottom, baseline).
  - `bgcolor`: Specifies the background color of the header.
  
**Use Case**: Grouping header rows to separate them from the body and footer of the table.

---

#### `<tbody>`

- **Description**: The `<tbody>` element groups the body content in a table.
- **Attributes**:
  - `align`: Specifies the alignment of the content in the body (left, center, right, justify).
  - `valign`: Specifies the vertical alignment of the content in the body (top, middle, bottom, baseline).
  - `bgcolor`: Specifies the background color of the body.
  
**Use Case**: Grouping rows that contain the main data of the table.

---

#### `<tfoot>`

- **Description**: The `<tfoot>` element groups the footer content in a table.
- **Attributes**:
  - `align`: Specifies the alignment of the content in the footer (left, center, right, justify).
  - `valign`: Specifies the vertical alignment of the content in the footer (top, middle, bottom, baseline).
  - `bgcolor`: Specifies the background color of the footer.
  
**Use Case**: Grouping footer rows to separate them from the body and header of the table.

---

#### `<colgroup>`

- **Description**: The `<colgroup>` element specifies a group of one or more columns in a table for formatting.
- **Attributes**:
  - `span`: Specifies the number of columns in the group.
  
**Use Case**: Applying styles or attributes to a group of columns.

---

#### `<col>`

- **Description**: The `<col>` element specifies column properties for each column within a `<colgroup>` element.
- **Attributes**:
  - `span`: Specifies the number of columns a `<col>` element should span.
  - `align`: Specifies the alignment of the content in the column (left, center, right, justify).
  - `valign`: Specifies the vertical alignment of the content in the column (top, middle, bottom, baseline).
  - `bgcolor`: Specifies the background color of the column.
  - `width`: Specifies the width of the column.
  
**Use Case**: Defining the properties of individual columns within a column group.

---

### Examples

Here is a basic example demonstrating the use of these elements:

```html
<table border="1" cellspacing="0" cellpadding="5">
  <caption>Sample Table</caption>
  <colgroup>
    <col span="2" style="background-color:lightgrey">
    <col style="background-color:lightgreen">
  </colgroup>
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
      <th>Header 3</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Data 1</td>
      <td>Data 2</td>
      <td>Data 3</td>
    </tr>
    <tr>
      <td>Data 4</td>
      <td>Data 5</td>
      <td>Data 6</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Footer 1</td>
      <td>Footer 2</td>
      <td>Footer 3</td>
    </tr>
  </tfoot>
</table>
```

In this example, we see the use of `<table>`, `<caption>`, `<colgroup>`, `<col>`, `<thead>`, `<tbody>`, `<tfoot>`, `<tr>`, `<th>`, and `<td>`. This table has a border, padding, and spacing specified, with a caption, and a column group that applies background colors to columns.

---

These elements and their attributes allow for the creation and styling of complex tables, making it easier to display structured data in a clear and organized manner.



Sure! Here are some interview questions about HTML tables along with solutions and examples using all the relevant tags and attributes.

---

### Question 1:
**Describe the structure of an HTML table and provide a complete example using `<table>`, `<th>`, `<tr>`, `<td>`, `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`, `<colgroup>`, and `<col>`. Include all possible attributes for each tag in your example.**

### Solution:

#### Explanation:
An HTML table is structured with rows (`<tr>`) and cells (`<td>` for data cells and `<th>` for header cells). A table can also include a caption (`<caption>`), and can be divided into a header (`<thead>`), body (`<tbody>`), and footer (`<tfoot>`). Columns can be grouped and styled using `<colgroup>` and `<col>`.

#### Example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Table Example</title>
</head>
<body>
    <table border="1" cellspacing="0" cellpadding="5" width="100%" height="200" align="center" bgcolor="lightyellow">
        <caption align="top">Sample Table with All Attributes</caption>
        
        <colgroup span="2">
            <col style="background-color:lightgrey" align="left" valign="middle" width="50%">
            <col style="background-color:lightblue" align="center" valign="top" width="50%">
        </colgroup>
        <colgroup>
            <col style="background-color:lightgreen" align="right" valign="bottom" width="100%">
        </colgroup>

        <thead align="center" valign="middle" bgcolor="lightcoral">
            <tr>
                <th scope="col" abbr="Header 1">Header 1</th>
                <th scope="col" abbr="Header 2">Header 2</th>
                <th scope="col" abbr="Header 3">Header 3</th>
            </tr>
        </thead>
        <tbody align="left" valign="top" bgcolor="lightgrey">
            <tr>
                <td headers="header1">Data 1</td>
                <td headers="header2">Data 2</td>
                <td headers="header3">Data 3</td>
            </tr>
            <tr>
                <td colspan="2" rowspan="2" headers="header1 header2">Data 4</td>
                <td headers="header3">Data 5</td>
            </tr>
            <tr>
                <td headers="header3">Data 6</td>
            </tr>
        </tbody>
        <tfoot align="right" valign="bottom" bgcolor="lightpink">
            <tr>
                <td headers="footer1">Footer 1</td>
                <td headers="footer2">Footer 2</td>
                <td headers="footer3">Footer 3</td>
            </tr>
        </tfoot>
    </table>
</body>
</html>
```

#### Explanation of Attributes:
- **`<table>` Attributes**:
  - `border`: Sets the border width of the table.
  - `cellpadding`: Sets the padding within each cell.
  - `cellspacing`: Sets the space between cells.
  - `width`: Sets the width of the table.
  - `height`: Sets the height of the table.
  - `align`: Sets the alignment of the table.
  - `bgcolor`: Sets the background color of the table.

- **`<caption>` Attributes**:
  - `align`: Sets the alignment of the caption.

- **`<colgroup>` Attributes**:
  - `span`: Specifies the number of columns the group should span.

- **`<col>` Attributes**:
  - `span`: Specifies the number of columns the element should span.
  - `align`: Sets the alignment of the column's content.
  - `valign`: Sets the vertical alignment of the column's content.
  - `bgcolor`: Sets the background color of the column.
  - `width`: Sets the width of the column.

- **`<thead>`, `<tbody>`, `<tfoot>` Attributes**:
  - `align`: Sets the alignment of the content.
  - `valign`: Sets the vertical alignment of the content.
  - `bgcolor`: Sets the background color.

- **`<th>` Attributes**:
  - `abbr`: Sets an abbreviated version of the content.
  - `scope`: Sets the scope of the header cell.
  - `colspan`: Sets the number of columns the header cell should span.
  - `rowspan`: Sets the number of rows the header cell should span.
  - `headers`: Specifies one or more header cells the cell is related to.

- **`<td>` Attributes**:
  - `colspan`: Sets the number of columns the cell should span.
  - `rowspan`: Sets the number of rows the cell should span.
  - `headers`: Specifies one or more header cells the cell is related to.
  - `align`: Sets the alignment of the cell's content.
  - `valign`: Sets the vertical alignment of the cell's content.
  - `bgcolor`: Sets the background color of the cell.

---

### Question 2:
**How can you create a table with merged cells using `colspan` and `rowspan` attributes? Provide an example.**

### Solution:

#### Explanation:
The `colspan` attribute is used to merge cells horizontally, and the `rowspan` attribute is used to merge cells vertically.

#### Example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Table with Merged Cells</title>
</head>
<body>
    <table border="1" cellspacing="0" cellpadding="5" width="100%" height="200" align="center" bgcolor="lightyellow">
        <caption align="top">Table with Merged Cells</caption>
        <thead>
            <tr>
                <th scope="col">Header 1</th>
                <th scope="col">Header 2</th>
                <th scope="col">Header 3</th>
                <th scope="col">Header 4</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td rowspan="2">Rowspan 2</td>
                <td>Data 2</td>
                <td>Data 3</td>
                <td>Data 4</td>
            </tr>
            <tr>
                <td colspan="3">Colspan 3</td>
            </tr>
            <tr>
                <td>Data 1</td>
                <td>Data 2</td>
                <td colspan="2">Colspan 2</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <td colspan="4">Footer</td>
            </tr>
        </tfoot>
    </table>
</body>
</html>
```

#### Explanation:
- **Row 1, Cell 1**: The `rowspan="2"` attribute makes this cell span two rows.
- **Row 2, Cell 2**: The `colspan="3"` attribute makes this cell span three columns.
- **Row 3, Cell 4**: The `colspan="2"` attribute makes this cell span two columns.
- **Footer Row**: The `colspan="4"` attribute makes this cell span four columns, covering the entire width of the table.

---

These examples and explanations should provide a solid understanding of how to use various HTML table tags and attributes in different scenarios.