# HTML Tables for Study Purposes

This README provides a brief explanation of HTML tables, their elements, attributes, and basic styling for study purposes.

## Table Elements
- **`<table>`**: Defines the table container.
- **`<tr>`**: Defines a table row.
- **`<td>`**: Defines a table data cell (standard cell).
- **`<th>`**: Defines a table header cell, typically bold and centered by default.

## Key Attributes
- **colspan**: Allows a cell to span multiple columns (e.g., `colspan="2"` spans two columns).
- **rowspan**: Allows a cell to span multiple rows (e.g., `rowspan="2"` spans two rows).
- **border**: Sets the table border thickness (e.g., `border="1"` for a visible border).
- **cellpadding**: Sets the space between cell content and borders (e.g., `cellpadding="5"`).
- **cellspacing**: Sets the space between cells (e.g., `cellspacing="5"`).

## Table Sections
- **`<thead>`**: Groups header content in a table.
- **`<tbody>`**: Groups the main body content of the table.
- **`<tfoot>`**: Groups footer content in a table, often for summaries.

## Basic Table Styling (CSS)
- **border-collapse**: Controls whether table borders are merged (`collapse`) or separated (`separate`).
  - Example: `border-collapse: collapse;`
- **width**: Sets the table or cell width (e.g., `width: 100%;` or `width: 200px;`).
- **height**: Sets the table or cell height (e.g., `height: 50px;`).

## Example Code
```html
<table border="1" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr>
      <th>Header 1</th>
      <th colspan="2">Header Spanning Two Columns</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Row 1, Cell 1</td>
      <td>Row 1, Cell 2</td>
      <td rowspan="2">Cell Spanning Two Rows</td>
    </tr>
    <tr>
      <td>Row 2, Cell 1</td>
      <td>Row 2, Cell 2</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="3">Footer spanning all columns</td>
    </tr>
  </tfoot>
</table>
```

## Notes
- Use CSS for modern styling instead of deprecated attributes like `border`, `cellpadding`, or `cellspacing`.
- Ensure tables are accessible by using `<th>` for headers and proper semantic structure.