# HTML

HTML (Hypertext Markup Language)

- It is a markup language which based on Standard Generalized Markup Language (SGML)
- SGML is a standard for specifying a markup language or tag set
- It define the structure of information on the Web page
- It doesn’t describe the actual presentation of a document
- It tells the web browser what content to display.
- Use a pre-defined set of tags to identify the webpage content types
- It is not a programming language

**Basic Structure of HTML Document**

```html
<!DOCTYPE> <!--Tell the browser the type of HTML standard
               Must appear first-->
<html>     
<head>     <!--Contain html document meta info, links, style
               sheet and scripts etc.               
               These are non web displayable info-->
     
<body>     <!--Contains the content that displays in the browser-->
</body>
</head>
</html>
```

---

---

### **Anatomy of HTML Elements/Tags**

```html
<!--Syntax:-->
<tag attribute = “Value”> Content </tag>

<a herf="contact.html">contact us </a>
<!--
from <...> opening tag
herf=".." = attribute
herf  = attribute name
contact.html = attribute value
contact us = content
</a> = closing tag
-->
```

HTML elements

- Represent some kind of structure
- It is a combination of a tag and its character data (content)
- HTML can be Empty element or Nested element also

Nested Element

- An element that contain other HTML elements

Empty Element

- An element with no character data (content)
- Also called Non-container tags or self closing tags
- Syntax: <self-closing-tag-name/>

HTML Tags

- Used to markup the text (content)
- Most of the tags come in as start and end tag pairs
- However, empty element tags doesn’t come in pairs
- The start tag may contain an attribute

HTML attributes

- Defines a property for an elements
- It is a way to describe the tags
- It must enclosed within the start tag
- It comes in a name/value pairs
- The value should enclosed within double quote
- An element can have one or more attributes
- Global attributes - common to all HTML el

### **Document structure elements**

```html
<META name="description" content="Free Web tutorials on HTML, CSS, XML, and XHTML" />
```

```html
<META name="keywords" content="HTML, DHTML, CSS, XML, XHTML, JavaScript" />
```

```html
<META http-equiv=“Refresh” content=“5;url=http://www.w3schools.com” />
```

```html
<META http-equiv="Content-Type" content=“text/html; charset=UTF-8” />
```

## **Text Markup Elements**

### **Heading elements**

```html
<h1>BIG</h1>
<h2></h2>
<h3></h3>
<h4></h4>   
<h5></h5>
<h6>small</h6>
```

### **Paragraph elements**

```html
<p> HTML element represents a paragraph</p>

<pre>- Represents preformatted text which is to be

presented exactly as written in the HTML file</pre>
```

### <br/>

- Represents a thematic break

### **<hr/>**

### **List elements**

- There are three main types of list in HTML, each one has a specific purpose

unordered list (<ul>)

ordered list(<ol>)

description list(<dd>)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>List Elements Example</title>
</head>
<body>

    <h1>List Elements Example</h1>

    <h2>Ordered List (ol)</h2>
    <ol>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
    </ol>

    <h2>Unordered List (ul)</h2>
    <ul>
        <li>Apple</li>
        <li>Orange</li>
        <li>Banana</li>
    </ul>

    <h2>Definition List (dl)</h2>
    <dl>
        <dt>HTML</dt>
        <dd>HyperText Markup Language</dd>

        <dt>CSS</dt>
        <dd>Cascading Style Sheets</dd>

        <dt>JS</dt>
        <dd>JavaScript</dd>
    </dl>

</body>
</html>
```

### **Text formatting elements**

- HTML provides several tags that you can use to make some text on

your web pages to appear differently than normal text

- Formatting elements were designed to display special types of text:

| Tag | Description |
| --- | --- |
| <b> | Defines bold text |
| <big> | Defines big text |
| <em> | Defines emphasized text |
| <i> | Defines italic text |
| <small> | Defines small text |
| <strong> | Defines strong text |

| Tag | Description |
| --- | --- |
| <sub> | Defines subscripted text |
| <sup> | Defines superscripted text |
| <s> | Renders text with a strike through but not important when indicating document edits |
| <u> | Deprecated. But in use for different purpose |

### **Demarcating and Quotation Elements**

| Tag | Description |
| --- | --- |
| <ins> | Defines inserted text |
| <del> | Defines deleted text |
| <mark> | Marked text |
| <samp> | sample output of a computer program |
| <code> | To show the computer code - Like a programming code |
| <kbd> | keyboard input text |
| <var> | To display the text as a variable - Like Programming variable |

### **comment(<!—hello—>)**

The syntax to add comments to your HTML source is as follow

```html
<!-- Write your comments goes here -->

```

### **Link elements**

```html
<a href="url">Link text</a>
```

### **Image ,** Audio and Video Elements

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Media Elements Example</title>
</head>
<body>

    <h1>Media Elements Example</h1>

    <!-- Image Element -->
    <h2>Image Element (img)</h2>
    <img src="https://via.placeholder.com/300" alt="Placeholder Image" width="300" height="200">

    <!-- Audio Element -->
    <h2>Audio Element (audio)</h2>
    <p>Press play to listen to a sample audio:</p>
    <audio controls>
        <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>

    <!-- Video Element -->
    <h2>Video Element (video)</h2>
    <p>Press play to watch a sample video:</p>
    <video width="400" height="300" controls>
        <source src="https://www.sample-videos.com/video123/mp4/720/big_buck_bunny_720p_1mb.mp4" type="video/mp4">
        Your browser does not support the video element.
    </video>

</body>
</html>
```

### Table Element

- The **`<table>`** element defines the table.
- The **`<thead>`** element contains the table header row (**`<tr>`**), and **`<th>`** elements define header cells.
- The **`<tbody>`** element contains the table body rows (**`<tr>`**), and **`<td>`** elements define data cells.
- The **`<tfoot>`** element contains the table footer row (**`<tr>`**), and **`<td>`** elements define footer cells.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Table Example</title>
</head>
<body>

    <h1>Table Example</h1>

    <!-- Table Element -->
    <table border="1">
        <!-- Table Header Row -->
        <thead>
            <tr>
                <!-- Header Cell 1 -->
                <th>Header 1</th>
                <!-- Header Cell 2 -->
                <th>Header 2</th>
                <!-- Header Cell 3 -->
                <th>Header 3</th>
            </tr>
        </thead>
        
        <!-- Table Body Rows -->
        <tbody>
            <!-- Row 1 -->
            <tr>
                <!-- Data Cell 1 -->
                <td>Row 1, Cell 1</td>
                <!-- Data Cell 2 -->
                <td>Row 1, Cell 2</td>
                <!-- Data Cell 3 -->
                <td>Row 1, Cell 3</td>
            </tr>
            
            <!-- Row 2 -->
            <tr>
                <!-- Data Cell 1 -->
                <td>Row 2, Cell 1</td>
                <!-- Data Cell 2 -->
                <td>Row 2, Cell 2</td>
                <!-- Data Cell 3 -->
                <td>Row 2, Cell 3</td>
            </tr>
        </tbody>
        
        <!-- Table Footer Row -->
        <tfoot>
            <tr>
                <!-- Footer Cell 1 -->
                <td colspan="3">Footer Content</td>
            </tr>
        </tfoot>
    </table>

</body>
</html>
```

### Form Element

The web form can contain one or more of the
following

<input> element

<textarea> element
• <button> element
• <select> element
• <option> element
• <optgroup> element
• <fieldset> element
• <legend> element
• <label> element
• <output> element
• <datalist> element
• <progress> element
• <meter> element<!--EndFragment-->
</body>
</html>

- The **`<form>`** element defines the web form and specifies the action ("/submit_form") and method ("post").
- Various form controls are included, such as text input, password input, radio buttons, a dropdown menu, checkboxes, and a textarea.
- Labels (**`<label>`**) are associated with their respective form controls to improve accessibility.
- The form includes a submit button (**`<input type="submit">`**) to submit the form data.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web Form Example</title>
</head>
<body>

    <h1>Web Form Example</h1>

    <!-- Form Element -->
    <form action="/submit_form" method="post">
        <!-- Text Input -->
        <label for="username">Username:</label>
        <input type="text" id="username" name="username" placeholder="Enter your username" required>
        <br>

        <!-- Password Input -->
        <label for="password">Password:</label>
        <input type="password" id="password" name="password" placeholder="Enter your password" required>
        <br>

        <!-- Radio Buttons -->
        <label>Gender:</label>
        <input type="radio" id="male" name="gender" value="male" checked>
        <label for="male">Male</label>
        <input type="radio" id="female" name="gender" value="female">
        <label for="female">Female</label>
        <br>

        <!-- Dropdown Menu -->
        <label for="country">Country:</label>
        <select id="country" name="country">
            <option value="usa">USA</option>
            <option value="canada">Canada</option>
            <option value="uk">UK</option>
        </select>
        <br>

        <!-- Checkboxes -->
        <label>Interests:</label>
        <input type="checkbox" id="music" name="interests" value="music">
        <label for="music">Music</label>
        <input type="checkbox" id="sports" name="interests" value="sports">
        <label for="sports">Sports</label>
        <br>

        <!-- Textarea -->
        <label for="message">Message:</label>
        <textarea id="message" name="message" placeholder="Enter your message"></textarea>
        <br>

        <!-- Submit Button -->
        <input type="submit" value="Submit">
    </form>

</body>
</html>
```

### HTML input types

1. **Text Input:**
    
    ```html
    htmlCopy code
    <input type="text" name="username" placeholder="Enter your username">
    
    ```
    
2. **Password Input:**
    
    ```html
    htmlCopy code
    <input type="password" name="password" placeholder="Enter your password">
    
    ```
    
3. **Checkbox:**
    
    ```html
    htmlCopy code
    <input type="checkbox" id="subscribe" name="subscribe" value="yes">
    <label for="subscribe">Subscribe to newsletter</label>
    
    ```
    
4. **Radio Buttons:**
    
    ```html
    htmlCopy code
    <input type="radio" id="male" name="gender" value="male">
    <label for="male">Male</label>
    <input type="radio" id="female" name="gender" value="female">
    <label for="female">Female</label>
    
    ```
    
5. **Dropdown Menu (Select):**
    
    ```html
    htmlCopy code
    <label for="country">Country:</label>
    <select id="country" name="country">
        <option value="usa">USA</option>
        <option value="canada">Canada</option>
        <option value="uk">UK</option>
    </select>
    
    ```
    
6. **File Input:**
    
    ```html
    htmlCopy code
    <input type="file" name="fileUpload">
    
    ```
    
7. **Submit Button:**
    
    ```html
    htmlCopy code
    <input type="submit" value="Submit">
    
    ```
    
8. **Reset Button:**
    
    ```html
    htmlCopy code
    <input type="reset" value="Reset">
    
    ```
    
9. **Hidden Input:**
    
    ```html
    htmlCopy code
    <input type="hidden" name="secretKey" value="someSecretValue">
    
    ```
    
10. **Date Input:**

```html
htmlCopy code
<input type="date" name="birthdate">

```

1. **Email Input:**

```html
htmlCopy code
<input type="email" name="userEmail" placeholder="Enter your email">

```

1. **Number Input:**

```html
htmlCopy code
<input type="number" name="quantity" min="1" max="10">

```

### range slider

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Range Slider Example</title>
    
</head>
<body>

    <h1>Range Slider Example</h1>

    <!-- Range Slider -->
    <label for="volume">Volume:</label>
    <input type="range" id="volume" name="volume" min="0" max="100" value="50">

    <!-- Display the selected value using CSS pseudo-elements -->
    <p>Selected Volume: <span id="volumeValue" data-value="50"></span></p>

</body>
</html>
```

### **GET Method:**

- **Purpose:** Used to request data from a specified resource.
- **Visibility:** Parameters are appended to the URL, visible in the browser's address bar.
- **Data Limitations:** Limited amount of data can be sent (URL length constraints).
- **Caching:** Can be cached, and the data is stored in the browser's history.
- **Security:** Not suitable for sensitive data like passwords, as data is visible in the URL.

Example:

```html
htmlCopy code
<form action="/search" method="get">
  <input type="text" name="query" placeholder="Search...">
  <input type="submit" value="Search">
</form>

```

- The form data is appended to the URL like: **`/search?query=search-term`**.

### **POST Method:**

- **Purpose:** Used to submit data to be processed to a specified resource.
- **Visibility:** Parameters are sent in the request body, not visible in the URL.
- **Data Limitations:** Can handle larger amounts of data compared to GET.
- **Caching:** Generally not cached, and the data is not stored in the browser's history.
- **Security:** More secure for sensitive data, as it's not visible in the URL.

Example:

```html
htmlCopy code
<form action="/submit_form" method="post">
  <input type="text" name="username" placeholder="Username">
  <input type="password" name="password" placeholder="Password">
  <input type="submit" value="Submit">
</form>

```

- The form data is sent in the request body, not visible in the URL.