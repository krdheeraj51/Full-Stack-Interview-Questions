## HTML Interview Questions

### 1. What is the difference between `<div>` and `<section>`?
Answer: `<div>` is a generic container, whereas `<section>` represents a thematic grouping.

### 2. How does the browser render CSS properties when multiple conflicting styles exist?
Answer: The browser resolves conflicts using **specificity**, **inheritance**, and **cascade** rules.

### 3. What are the new features introduced in HTML5?
Answer: HTML5 introduced several new features that enhance web development, making it more dynamic and interactive. Here are some key additions:

1. **Audio and Video Support** – The `<audio>` and `<video>` tags allow embedding multimedia content without requiring third-party plugins like Flash.
2. **Canvas and SVG Graphics** – Enables drawing graphics, animations, and interactive elements directly within the browser using JavaScript.
3. **Semantic Elements** – New tags like `<header>`, `<footer>`, `<article>`, and `<section>` improve readability and accessibility.
4. **Local Storage and IndexedDB** – Provides better offline storage capabilities compared to cookies.
5. **Geolocation API** – Allows websites to access a user's location with their permission.
6. **Web Workers** – Enables background processing for improved performance.
7. **Drag and Drop API** – Simplifies drag-and-drop functionality for web applications.
8. **Form Enhancements** – New input types like `email`, `date`, `number`, and `range` improve user experience.

### 4. What is difference between <div> and <span>?
Answer: The `<div>` and `<span>` elements in HTML serve different purposes:

1. **`<div>` (Block-level element)**:
   - Used to group and structure content into sections.
   - Takes up the full width available.
   - Commonly used for layout and styling purposes.
   - Example:
     ```html
     <div style="background-color:lightblue;">
       <h2>Welcome to My Website</h2>
       <p>This is a section of content.</p>
     </div>
     ```

2. **`<span>` (Inline element)**:
   - Used to style or manipulate specific portions of text within a block.
   - Does not create a new section or take up full width.
   - Example:
     ```html
     <p>This is <span style="color:red;">important</span> text.</p>
     ```

In short, `<div>` is for **structuring** larger sections, while `<span>` is for **styling** smaller portions within a block. Would you like more examples or best practices for using them?

### 5. What is the Purpose of the <!DOCTYPE> declaration in HTML?
Answer: The <!DOCTYPE> declaration is used to specify the document type and version of HTML being used. It helps the browser understand how to render the web page correctly.

### 6. What are data attributes in HTML?
Answer: Data attributes in HTML allow developers to store custom data directly within HTML elements. They are useful for embedding extra information that can be accessed via JavaScript or CSS without requiring additional database queries or AJAX calls.

### Key Features:
1. **Custom Data Storage** – Data attributes start with `data-` and can hold any string value.
2. **JavaScript Access** – You can retrieve data attributes using `element.dataset` in JavaScript.
3. **CSS Styling** – Data attributes can be used in CSS selectors for styling elements dynamically.

### Example:
```html
<button data-user-id="12345" data-role="admin">Click Me</button>
```
Accessing the data in JavaScript:
```javascript
const button = document.querySelector("button");
console.log(button.dataset.userId); // Output: "12345"
console.log(button.dataset.role); // Output: "admin"
```

...