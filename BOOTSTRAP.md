# BOOTSTRAP

# **Getting Started:**

1. **Include Bootstrap:**
You can include Bootstrap in your project by adding the following CDN link to your HTML file:
    
    ```html
    
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css">
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"></script>
    
    ```
    
2. **Start Using Components:**
Once Bootstrap is included, you can start using its components and styles in your HTML.
    
    Example:
    
    ```html
    
    <div class="container">
        <h1 class="display-4">Hello, Bootstrap!</h1>
        <button class="btn btn-success">Click me</button>
    </div>
    
    ```
    

# **Bootstrap Containers**

In this tutorial you will learn how to create containers with Bootstrap.

# **Creating Containers with Bootstrap**

Containers are the most basic layout element in Bootstrap and are required when using the grid system. Containers are basically used to wrap content with some padding. They are also used to align the content horizontally center on the page in case of fixed width layout.

 three different types containers:

- `.container`, which has a max-width at each responsive breakpoint.
- `.container-fluid`, which has 100% width at all breakpoints.
- `.container-{breakpoint}`, which has 100% width until the specified breakpoint.

```html
<div class="container">
    <h1>This is a heading</h1>
    <p>This is a paragraph of text.</p>
</div>
```

example :width of the container will change at different breakpoints or screen sizes, as shown above.

### **Fluid Containers**

You can use the `.container-fluid` class to create a full width container. The width of the fluid container will always be 100% irrespective of the devices or screen sizes.

```markup
<div class="container-fluid"><h1>This is a heading</h1><p>This is a paragraph of text.</p></div>
```

### **Specify Responsive Breakpoints for Containers**

Since Bootstrap v4.4, you can also create containers that is 100% wide until the specified breakpoint is reached, after which max-width for each of the higher breakpoints will be applied.

```markup
<div class="container-sm">100% wide until screen size less than 576px</div><div class="container-md">100% wide until screen size less than 768px</div><div class="container-lg">100% wide until screen size less than 992px</div><div class="container-xl">100% wide until screen size less than 1200px</div>
```

---

### **Adding Background and Borders to Containers**

By default, container doesn't have any `[background-color](https://www.tutorialrepublic.com/css-reference/css-background-color-property.php)` or `[border](https://www.tutorialrepublic.com/css-reference/css-color-property.php)`. But if you need you can apply your own styles, or simply use the Bootstrap background-color and border [utility classes](https://www.tutorialrepublic.com/twitter-bootstrap-tutorial/bootstrap-helper-classes.php) to add background-color or border on them, as shown in the following example.

```markup
<!-- Container with dark background and white text color -->
<div class="container bg-dark text-white"><h1>This is a heading</h1><p>This is a paragraph of text.</p></div><!-- Container with light background -->
<div class="container bg-light"><h1>This is a heading</h1><p>This is a paragraph of text.</p></div><!-- Container with border -->
<div class="container border"><h1>This is a heading</h1><p>This is a paragraph of text.</p></div>
```

---

### **Applying Paddings and Margins to Containers**

By default, containers have padding of 12px on the left and right sides, and no padding on the top and bottom sides. To apply extra padding and margins you can use the [spacing utility classes](https://www.tutorialrepublic.com/twitter-bootstrap-tutorial/bootstrap-helper-classes.php).

```markup
<!-- Container with border, extra paddings and margins -->
<div class="container border py-3 my-3"><h1>This is a heading</h1><p>This is a paragraph of text.</p></div>
```

### **Navbar:**

The Navbar component in Bootstrap provides a responsive navigation bar that adapts to different screen sizes.

```html

<nav class="navbar navbar-expand-lg navbar-light bg-light">
    <a class="navbar-brand" href="#">Logo</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ml-auto">
            <li class="nav-item active">
                <a class="nav-link" href="#">Home</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#">About</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#">Services</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#">Contact</a>
            </li>
        </ul>
    </div>
</nav>

```

This example creates a responsive Navbar with a brand logo and navigation links.

### **Jumbotron:**

The Jumbotron component is used for showcasing key content or messages prominently.

```html

<div class="jumbotron">
    <h1 class="display-4">Welcome to our Website!</h1>
    <p class="lead">Discover the best of what we have to offer.</p>
    <hr class="my-4">
    <p>Explore our services and learn more about us.</p>
    <a class="btn btn-primary btn-lg" href="#" role="button">Get Started</a>
</div>

```

This Jumbotron example creates a visually appealing section with a heading, lead text, and a call-to-action button.

### **Cards:**

Bootstrap Cards are versatile containers that can hold various types of content.

```html

<div class="card" style="width: 18rem;">
    <img src="https://via.placeholder.com/150" class="card-img-top" alt="Card Image">
    <div class="card-body">
        <h5 class="card-title">Card Title</h5>
        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        <a href="#" class="btn btn-primary">Learn More</a>
    </div>
</div>

```

This Card example includes an image, a title, text, and a button.

### **Alerts:**

Bootstrap Alerts provide a way to communicate important messages to users.

```html

<div class="alert alert-success" role="alert">
    This is a success alert!
</div>

```

This example creates a success alert. Bootstrap provides various alert styles, including success, info, warning, and danger.

### **Forms:**

Bootstrap simplifies the creation of stylish and responsive forms.

```html

<form>
    <div class="form-group">
        <label for="exampleInputEmail1">Email address</label>
        <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email">
        <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
    </div>
    <div class="form-group">
        <label for="exampleInputPassword1">Password</label>
        <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
</form>

```

This example creates a simple form with email and password fields.

### **Modals:**

Bootstrap Modals are used to display content or prompts on top of the current page.

```html

<!-- Button trigger modal -->
<button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
    Launch Modal
</button>

<!-- Modal -->
<div class="modal fade" id="exampleModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog" role="document">
        <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title" id="exampleModalLabel">Modal Title</h5>
                <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                    <span aria-hidden="true">&times;</span>
                </button>
            </div>
            <div class="modal-body">
                Content goes here.
            </div>
            <div class="modal-footer">
                <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
                <button type="button" class="btn btn-primary">Save changes</button>
            </div>
        </div>
    </div>
</div>

```

This example demonstrates a button triggering a modal with a title, content, and footer buttons.

### **Bootstrap Overview:**

Bootstrap is a popular open-source front-end framework that facilitates the development of responsive, mobile-first web projects. It includes a set of pre-designed components, utilities, and styles that developers can leverage to create consistent and visually appealing user interfaces.

### **Key Features:**

1. **Responsive Grid System:**
Bootstrap uses a responsive grid system with 12 columns, making it easy to create flexible and responsive layouts. Columns can be adjusted based on the device screen size.
    
    Example:
    
    ```html
    
    <div class="container">
        <div class="row">
            <div class="col-md-6">Column 1</div>
            <div class="col-md-6">Column 2</div>
        </div>
    </div>
    
    ```
    
2. **Pre-designed Components:**
Bootstrap offers a variety of ready-to-use components such as navigation bars, buttons, forms, modals, and more. These components can be easily customized and integrated into your project.
    
    Example:
    
    ```html
    
    <button class="btn btn-primary">Primary Button</button>
    
    ```
    
3. **Responsive Typography:**
Bootstrap provides a flexible and customizable typography system, ensuring text is easily readable on all devices.
    
    Example:
    
    ```html
    
    <h1 class="display-4">Heading</h1>
    <p class="lead">This is a lead paragraph.</p>
    
    ```
    
4. **CSS Flexbox and Grid Utilities:**
Bootstrap includes utility classes for Flexbox and Grid layout, allowing developers to quickly create responsive and dynamic layouts.
    
    Example:
    
    ```html
    
    <div class="d-flex justify-content-between">
        <div>Item 1</div>
        <div>Item 2</div>
    </div>
    
    ```
    
5. **JavaScript Plugins:**
Bootstrap comes with JavaScript plugins for common UI components like carousels, modals, tooltips, and more. These plugins enhance the functionality of your web pages.
    
    Example (Modal):
    
    ```html
    
    <button type="button" class="btn btn-primary" data-toggle="modal" data-target="#myModal">
        Open Modal
    </button>
    
    <div class="modal" id="myModal">
        <div class="modal-dialog">
            <div class="modal-content">
                <!-- Modal content -->
            </div>
        </div>
    </div>
    
    ```
    

### **Customization:**

Bootstrap can be customized by overriding its default styles and components. You can create a custom stylesheet to modify colors, fonts, and other styles to match your project's design.

Bootstrap provides extensive documentation that covers all its features, components, and customization options. You can find more details in the official Bootstrap documentation.

Bootstrap is a powerful tool for quickly building responsive and visually appealing web applications. It's widely used in the web development community, and its extensive ecosystem of themes and plugins makes it a go-to choice for many developers.

### **Cards:**

**Definition:**
Bootstrap Cards are a flexible and extensible content container. They include options for headers, footers, images, and various content types.

**Example:**

```html

<div class="card" style="width: 18rem;">
    <img src="https://via.placeholder.com/150" class="card-img-top" alt="Card Image">
    <div class="card-body">
        <h5 class="card-title">Card Title</h5>
        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        <a href="#" class="btn btn-primary">Learn More</a>
    </div>
</div>

```

### **Tables:**

**Definition:**
Bootstrap Tables provide a way to display tabular data with features like striped rows, responsive design, and hover effects.

**Example:**

```html

<table class="table">
    <thead>
        <tr>
            <th scope="col">#</th>
            <th scope="col">First Name</th>
            <th scope="col">Last Name</th>
            <th scope="col">Age</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope="row">1</th>
            <td>John</td>
            <td>Doe</td>
            <td>25</td>
        </tr>
        <tr>
            <th scope="row">2</th>
            <td>Jane</td>
            <td>Smith</td>
            <td>30</td>
        </tr>
    </tbody>
</table>

```

### **Flex:**

**Definition:**
Flexbox, or the Flexible Box Layout, is a one-dimensional layout method for laying out items in rows or columns. It provides a more efficient and predictable way to distribute space among items in a container.

**Example:**

```html

<div class="d-flex justify-content-between">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>

```

### **Forms:**

**Definition:**
Bootstrap Forms simplify the process of creating responsive and visually appealing forms. They include various form controls and styling options.

**Example:**

```html

<form>
    <div class="form-group">
        <label for="exampleInputEmail1">Email address</label>
        <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email">
        <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
    </div>
    <div class="form-group">
        <label for="exampleInputPassword1">Password</label>
        <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
</form>

```

### **Drop-downs:**

**Definition:**
Bootstrap Drop-downs are toggleable, contextual overlays that provide additional navigation or content options.

**Example:**

```html

<div class="dropdown">
    <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        Dropdown button
    </button>
    <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
        <a class="dropdown-item" href="#">Action</a>
        <a class="dropdown-item" href="#">Another action</a>
        <a class="dropdown-item" href="#">Something else here</a>
    </div>
</div>

```

### **Collapse:**

**Definition:**
Bootstrap Collapse provides a way to toggle the visibility of content. It is often used in conjunction with navigation components.

**Example:**

```html

<button class="btn btn-primary" type="button" data-toggle="collapse" data-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
    Toggle Content
</button>

<div class="collapse" id="collapseExample">
    <div class="card card-body">
        This is the collapsible content.
    </div>
</div>

```

### **Buttons:**

**Definition:**
Bootstrap provides a variety of button styles and options to enhance the user interface. Buttons can have different colors, sizes, and states.

**Examples:**

```html

<button type="button" class="btn btn-primary">Primary Button</button>
<button type="button" class="btn btn-secondary">Secondary Button</button>
<button type="button" class="btn btn-success">Success Button</button>
<button type="button" class="btn btn-danger">Danger Button</button>
<button type="button" class="btn btn-warning">Warning Button</button>
<button type="button" class="btn btn-info">Info Button</button>
<button type="button" class="btn btn-light">Light Button</button>
<button type="button" class="btn btn-dark">Dark Button</button>
<button type="button" class="btn btn-outline-primary">Outline Primary</button>

```

**Description:**

- The **`btn`** class is used to define a Bootstrap button.
- **`btn-primary`**, **`btn-secondary`**, etc., classes define different button color variations.
- **`btn-outline-primary`** creates a primary button with an outlined appearance.

### **Spinners:**

**Definition:**
Bootstrap Spinners provide animated loading indicators. They are useful when waiting for content to load or an action to complete.

**Examples:**

```html

<div class="spinner-border" role="status">
    <span class="sr-only">Loading...</span>
</div>

<div class="spinner-border text-primary" role="status">
    <span class="sr-only">Loading...</span>
</div>

<div class="spinner-border text-success" role="status">
    <span class="sr-only">Loading...</span>
</div>

<div class="spinner-border text-danger" role="status">
    <span class="sr-only">Loading...</span>
</div>

<div class="spinner-border text-warning" role="status">
    <span class="sr-only">Loading...</span>
</div>

```

**Description:**

- The **`spinner-border`** class creates a basic spinner.
- **`text-primary`**, **`text-success`**, etc., classes define different spinner color variations.
- The **`sr-only`** class is used for screen reader accessibility by visually hiding the loading text.