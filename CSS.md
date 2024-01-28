# CSS

• CSS describes how HTML elements are to be displayed on screen, paper, or in other media

# Three Ways to Insert CSS

There are three ways of inserting a style sheet:

- External CSS
- Internal CSS
- Inline CSS

---

# External CSS

With an external style sheet, you can change the look of an entire website by changing just one file!

Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.

# Example

External styles are defined within the <link> element, inside the <head> section of an HTML page:

```html
<!DOCTYPE html>
<html><head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>
<h1>This is a heading</h1>
<p>This is a paragraph.</p>
</body></html>
```

An external style sheet can be written in any text editor, and must be saved with a .css extension.

The external .css file should not contain any HTML tags.

Here is how the "mystyle.css" file looks:

# "mystyle.css"

```css
body { 
 background-color: lightblue;
}
h1 {  
color: navy;  margin-left: 20px;
}
```

# Internal CSS

An internal style sheet may be used if one single HTML page has a unique style.

The internal style is defined inside the <style> element, inside the head section.

# Example

Internal styles are defined within the <style> element, inside the <head> section of an HTML page:

```html
<!DOCTYPE html>
<html><head>
<style>
body {  background-color: linen;}
h1 {  color: maroon;  margin-left: 40px;}
</style>
</head><body>
<h1>This is a heading</h1>
<p>This is a paragraph.</p>
</body></html>
```

# Inline CSS

An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

# Example

Inline styles are defined within the "style" attribute of the relevant element:

```html
<!DOCTYPE html>
<html><body>
<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>
</body></html>
```

classes and IDs are selectors that allow you to target and style specific HTML elements. Here's how you can use them with examples:

### **1. Using Classes:**

### HTML:

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Class Example</title>
</head>
<body>
    <div class="box blue">Blue Box</div>
    <div class="box red">Red Box</div>
    <div class="box green">Green Box</div>
</body>
</html>

```

### CSS (styles.css):

```css

/* Target elements with the class 'box' */
.box {
    width: 100px;
    height: 100px;
    text-align: center;
    line-height: 100px;
    margin: 10px;
}

/* Specific styles for each color class */
.blue {
    background-color: #3498db;
    color: #fff;
}

.red {
    background-color: #e74c3c;
    color: #fff;
}

.green {
    background-color: #2ecc71;
    color: #fff;
}

```

### **2. Using IDs:**

### HTML:

```html
htmlCopy code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>ID Example</title>
</head>
<body>
    <div id="header">Header Section</div>
    <div id="main-content">Main Content</div>
    <div id="footer">Footer Section</div>
</body>
</html>

```

### CSS (styles.css):

```css

/* Target elements with the ID 'header' */
#header {
    background-color: #333;
    color: #fff;
    padding: 10px;
}

/* Target elements with the ID 'main-content' */
#main-content {
    background-color: #ecf0f1;
    padding: 20px;
}

/* Target elements with the ID 'footer' */
#footer {
    background-color: #333;
    color: #fff;
    padding: 10px;
}

```

### **Key Points:**

- **Classes:**
    - Used to style multiple elements with the same class.
    - Apply styles to elements using **`.className`** in CSS.
    - Elements can have multiple classes: **`<div class="box blue">`**.
- **IDs:**
    - Should be unique within a page.
    - Apply styles to an element using **`#idName`** in CSS.
    - Elements should only have one ID: **`<div id="header">`**.

Remember, IDs should be unique, and classes can be applied to multiple elements. Choose between them based on your specific styling needs. If you need to apply a style to multiple elements, use a class; if it's a unique element, use an ID.

### **CSS Examples and Descriptions**

### **Basic Styling:**

```css

body {
    font-family: 'Arial', sans-serif;
    background-color: #f0f0f0;
    color: #333;
}

h1 {
    color: #009688;
}

p {
    line-height: 1.5;
}

```

- **Description:** Sets the font family for the entire document, defines a background color, and sets default text color. Adjusts the color of **`h1`** elements and sets a comfortable line height for **`p`** elements.

### **Box Model:**

```css

.box {
    width: 200px;
    height: 150px;
    padding: 20px;
    margin: 10px;
    border: 2px solid #333;
    background-color: #fff;
}

```

- **Description:** Defines a box with specified width and height, adds padding inside the box, sets margins around the box, applies a border, and sets a background color.

### **Flexbox Layout:**

```css

.flex-container {
    display: flex;
    justify-content: space-between;
}

.flex-item {
    flex: 1;
    margin: 10px;
}

```

- **Description:** Creates a flex container with items spaced evenly. Each flex item takes equal space within the container and has a margin.

### **Responsive Design:**

```css

@media (max-width: 768px) {
    .responsive-image {
        max-width: 100%;
        height: auto;
    }
}

```

- **Description:** Makes images responsive by setting a maximum width of 100% when the screen width is 768 pixels or less.

### Responsive Font Size:

```css

/* CSS Media Query Example for Responsive Font Size */
@media screen and (max-width: 768px) {
    .responsive-text {
        font-size: 14px;
    }
}

@media screen and (min-width: 769px) and (max-width: 1024px) {
    .responsive-text {
        font-size: 16px;
    }
}

```

This example demonstrates a media query adjusting the font size based on different screen widths, providing a responsive design.

### Responsive Grid Layout:

```css

/* CSS Media Query Example for Responsive Grid Layout */
@media screen and (max-width: 600px) {
    .grid-container {
        grid-template-columns: 1fr; /* Adjust the grid to a single column layout */
    }
}

```

This example uses a media query to modify the grid layout for smaller screens, changing the number of columns.

### **Animation:**

```css

.animated-text {
    animation: fadeIn 2s ease-in-out;
}

@keyframes fadeIn {
    0% { opacity: 0; }
    100% { opacity: 1; }
}

```

- **Description:** Animates the opacity of an element to create a fadeIn effect over 2 seconds.

### **Dropdown Menu:**

```css

.dropdown {
    position: relative;
    display: inline-block;
}

.dropdown-content {
    display: none;
    position: absolute;
    background-color: #f9f9f9;
}

.dropdown:hover .dropdown-content {
    display: block;
}

```

- **Description:** Creates a simple CSS-only dropdown menu with hover effect.

### **Gradient Background:**

```css

.gradient-background {
    background: linear-gradient(to right, #ff8c00, #ff0080);
    color: #fff;
}

```

- **Description:** Applies a gradient background from orange to pink with white text.

### **Hover Effects:**

```css

.hover-effect {
    transition: transform 0.3s ease-in-out;
}

.hover-effect:hover {
    transform: scale(1.1);
}

```

- **Description:** Adds a scaling effect to an element when hovered.

### **Custom Fonts:**

```css

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

body {
    font-family: 'Roboto', sans-serif;
}

```

- **Description:** Imports and applies the Roboto font to the entire document.

### **Dark Mode:**

```css

body.dark-mode {
    background-color: #333;
    color: #fff;
}

```

- **Description:** Styles for implementing a dark mode by changing background and text colors.

The CSS **`display`** property is used to define how an HTML element should be displayed. Here are some common values for the **`display`** property along with examples:

### **1. Block:**

```css

.block-example {
    display: block;
}

```

This makes the element a block-level element, starting on a new line and taking up the full width.

### **2. Inline:**

```css

.inline-example {
    display: inline;
}

```

This makes the element an inline-level element, allowing it to flow with the content and only taking up as much width as necessary.

### **3. Inline-Block:**

```css

.inline-block-example {
    display: inline-block;
}

```

This makes the element an inline-level block container. It behaves like an inline element, but it can have a width and height.

### **4. None:**

```css

.none-example {
    display: none;
}

```

This hides the element. The element will be invisible and won't take up any space.

### **5. Flex:**

```css

.flex-example {
    display: flex;
}

```

This establishes a flex container, enabling flex properties for its direct children.

### Flex Container Properties:

```css

/* CSS Flex Container Example */
.flex-container {
    display: flex;
    flex-direction: row; /* or column-reverse, row-reverse, etc. */
    justify-content: space-around; /* or flex-start, flex-end, space-between, space-around, space-evenly */
    align-items: center; /* or flex-start, flex-end, baseline, stretch */
    flex-wrap: wrap; /* or nowrap, wrap-reverse */
}

```

This example demonstrates various properties for a flex container, controlling the direction, justification, alignment, and wrapping of flex items.

### Flex Items:

```css

/* CSS Flex Items Example */
.flex-item {
    flex: 1; /* or a specific value */
    order: 2; /* Change the order of a specific item */
    align-self: flex-end; /* or flex-start, center, baseline, stretch */
}

```

This example showcases properties for individual flex items within the flex container, adjusting their flexibility, order, and alignment.

### **6. Grid:**

```css

.grid-example {
    display: grid;
}

```

This establishes a grid container, enabling grid properties for its direct children.

### **Example HTML:**

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>CSS Display Example</title>
</head>
<body>
    <div class="block-example">Block Example</div>
    <span class="inline-example">Inline Example</span>
    <div class="inline-block-example">Inline-Block Example</div>
    <div class="none-example">None Example (Hidden)</div>
    <div class="flex-example">
        <div>Flex Item 1</div>
        <div>Flex Item 2</div>
        <div>Flex Item 3</div>
    </div>
    <div class="grid-example">
        <div>Grid Item 1</div>
        <div>Grid Item 2</div>
        <div>Grid Item 3</div>
    </div>
</body>
</html>

```

### **Example CSS (styles.css):**

```css

body {
    font-family: 'Arial', sans-serif;
    text-align: center;
}

div, span {
    margin: 10px;
    padding: 10px;
    border: 1px solid #333;
}

.none-example {
    color: red; /* Text color to show that it's hidden */
    display: none;
}

.flex-example, .grid-example {
    display: flex;
    gap: 10px;
}

.grid-example {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
}

```

### Grid Container Properties:

```css

/* CSS Grid Container Example */
.grid-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* Create a 3-column grid */
    grid-template-rows: auto; /* or specific values like 100px 200px */
    gap: 10px; /* Add a gap between grid items */
    justify-content: center; /* or start, end, space-between, space-around, space-evenly */
    align-items: center; /* or start, end, center, stretch */
}

```

This example showcases properties for a grid container, defining the columns, rows, gap, justification, and alignment.

### Grid Items:

```css
cssCopy code
/* CSS Grid Items Example */
.grid-item {
    grid-column: span 2; /* or a specific value */
    grid-row: 1 / span 2; /* or a specific value */
}

```

This example illustrates properties for individual grid items within the grid container, specifying their column and row spans.

The CSS **`cursor`** property allows you to customize the appearance of the cursor when it hovers over an element. Here are some common cursor values along with examples:

### **1. Default Cursor:**

```css

.default-cursor {
    cursor: default;
}

```

This sets the default cursor, usually an arrow.

### **2. Pointer Cursor:**

```css

.pointer-cursor {
    cursor: pointer;
}

```

This changes the cursor to a pointing hand, indicating a link or interactive element.

### **3. Crosshair Cursor:**

```css

.crosshair-cursor {
    cursor: crosshair;
}

```

This changes the cursor to a crosshair, indicating a selection or target area.

### **4. Text Cursor:**

```css

.text-cursor {
    cursor: text;
}

```

This changes the cursor to a text input cursor, indicating text can be selected or edited.

### **5. Move Cursor:**

```css

.move-cursor {
    cursor: move;
}

```

This changes the cursor to a four-sided arrow, indicating that the element can be moved.

### **6. Resize Cursor:**

```css

.resize-cursor {
    cursor: ew-resize;
}

```

This changes the cursor to a horizontal resize arrow, indicating the element can be resized horizontally.

### **7. Not-allowed Cursor:**

```css

.not-allowed-cursor {
    cursor: not-allowed;
}

```

This changes the cursor to a circle with a line through it, indicating that the action is not allowed.

### **8. Help Cursor:**

```css

.help-cursor {
    cursor: help;
}

```

This changes the cursor to a question mark, indicating that the user can get help.

### **Example HTML:**

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>CSS Cursor Example</title>
</head>
<body>
    <div class="default-cursor">Default Cursor</div>
    <div class="pointer-cursor">Pointer Cursor</div>
    <div class="crosshair-cursor">Crosshair Cursor</div>
    <div class="text-cursor">Text Cursor</div>
    <div class="move-cursor">Move Cursor</div>
    <div class="resize-cursor">Resize Cursor</div>
    <div class="not-allowed-cursor">Not Allowed Cursor</div>
    <div class="help-cursor">Help Cursor</div>
</body>
</html>

```

### **Example CSS (styles.css):**

```css

body {
    font-family: 'Arial', sans-serif;
    text-align: center;
}

div {
    margin: 20px;
    padding: 10px;
    border: 1px solid #333;
}

.default-cursor {
    cursor: default;
}

.pointer-cursor {
    cursor: pointer;
}

.crosshair-cursor {
    cursor: crosshair;
}

.text-cursor {
    cursor: text;
}

.move-cursor {
    cursor: move;
}

.resize-cursor {
    cursor: ew-resize;
}

.not-allowed-cursor {
    cursor: not-allowed;
}

.help-cursor {
    cursor: help;
}

```

### **Background:**

### HTML:

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Background Example</title>
</head>
<body>
    <div class="background-example">
        <h1>Background Example</h1>
    </div>
</body>
</html>

```

### CSS (styles.css):

```css

/* Background styling */
.background-example {
    background-color: #3498db; /* Background color */
    color: #fff; /* Text color */
    padding: 20px; /* Padding inside the box */
}

```

### **Border:**

### HTML:

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Border Example</title>
</head>
<body>
    <div class="border-example">
        <h1>Border Example</h1>
    </div>
</body>
</html>

```

### CSS (styles.css):

```css

/* Border styling */
.border-example {
    border: 2px solid #e74c3c; /* Border with color */
    padding: 20px; /* Padding inside the box */
}

```

### **Box Model:**

### HTML:

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Box Model Example</title>
</head>
<body>
    <div class="box-model-example">
        <h1>Box Model Example</h1>
    </div>
</body>
</html>

```

### CSS (styles.css):

```css

/* Box Model styling */
.box-model-example {
    width: 300px; /* Width of the box */
    height: 150px; /* Height of the box */
    margin: 20px; /* Margin outside the box */
    padding: 20px; /* Padding inside the box */
    border: 2px solid #2ecc71; /* Border with color */
}

```

### **Text:**

### HTML:

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Text Example</title>
</head>
<body>
    <div class="text-example">
        <p>This is a styled text example.</p>
    </div>
</body>
</html>

```

### CSS (styles.css):

```css

/* Text styling */
.text-example {
    font-family: 'Arial', sans-serif; /* Font family */
    font-size: 18px; /* Font size */
    font-weight: bold; /* Font weight */
    color: #333; /* Text color */
    line-height: 1.5; /* Line height */
}

```

### **Box Shadow:**

### HTML:

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Box Shadow Example</title>
</head>
<body>
    <div class="box-shadow-example">
        <h1>Box Shadow Example</h1>
    </div>
</body>
</html>

```

### CSS (styles.css):

```css

/* Box Shadow styling */
.box-shadow-example {
    width: 200px; /* Width of the box */
    height: 100px; /* Height of the box */
    background-color: #3498db; /* Background color */
    box-shadow: 5px 5px 10px #888888; /* Box shadow with offsets, blur radius, and color */
    padding: 20px; /* Padding inside the box */
    color: #fff; /* Text color */
}

```

### **Icons:**

```css

/* CSS Icon Example */
.icon-example {
    font-family: 'Font Awesome 5 Free'; /* Assume Font Awesome is imported */
    content: '\f007'; /* Unicode for a specific icon */
    font-size: 24px;
    color: #3498db;
}

```

This example uses Font Awesome to display an icon. Adjust the Unicode and font size based on the icon and design preferences.

### **Lists:**

```css

/* CSS List Example */
.list-example {
    list-style-type: disc; /* Type of bullet (circle) */
    margin-left: 20px; /* Indentation */
}

```

This example styles an unordered list with disc bullets and an indentation of 20 pixels.

### **Letter Spacing:**

```css

/* CSS Letter Spacing Example */
.letter-spacing-example {
    letter-spacing: 2px; /* Adjust letter spacing */
}

```

This example increases the letter spacing between characters by 2 pixels.

### **Text Indent:**

```css

/* CSS Text Indent Example */
.text-indent-example {
    text-indent: 20px; /* Adjust the indentation of the first line */
}

```

This example indents the first line of text by 20 pixels.

### **Text Stroke:**

```css

/* CSS Text Stroke Example */
.text-stroke-example {
    -webkit-text-stroke: 1px #000; /* Text stroke width and color for WebKit browsers */
    text-stroke: 1px #000; /* Text stroke width and color for non-WebKit browsers */
}

```

This example adds a 1-pixel stroke to the text with a black color.

### **Order:**

```css

/* CSS Order Example */
.order-example {
    order: 2; /* Change the order of a flex item */
}

```

This example changes the order of a flex item to be displayed second.

### **Superscript and Subscript:**

```css

/* CSS Superscript and Subscript Example */
.superscript-example {
    vertical-align: super; /* Display text as superscript */
}

.subscript-example {
    vertical-align: sub; /* Display text as subscript */
}

```

These examples adjust the vertical alignment to display text as superscript or subscript.