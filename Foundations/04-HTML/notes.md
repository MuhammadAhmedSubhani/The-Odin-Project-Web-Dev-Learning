# HTML – Complete Study Notes
## The Odin Project | Foundations

**Subject:** HyperText Markup Language (HTML)  
**Learning Resource:** The Odin Project  
**Level:** Beginner / Foundations  
**Purpose:** Exam Preparation, Revision and Practical Reference

---

# Table of Contents

1. Introduction to HTML
2. HTML vs CSS vs JavaScript
3. HTML Elements and Tags
4. HTML Attributes
5. HTML Boilerplate
6. HTML Document Structure
7. Working with Text
8. HTML Headings
9. Paragraphs
10. Bold and Italic Text
11. HTML Nesting and Indentation
12. HTML Comments
13. HTML Lists
14. Unordered Lists
15. Ordered Lists
16. Nested Lists
17. HTML Links
18. Absolute and Relative Links
19. HTML Images
20. Image Attributes
21. File Paths
22. Semantic HTML – Additional Knowledge
23. HTML Validation and Common Errors
24. The Odin Project: Recipes Project
25. Important HTML Tags Reference
26. Common Mistakes
27. Exam Preparation Questions
28. Practical Exercises
29. Quick Revision Sheet

---

# 1. Introduction to HTML

## 1.1 What is HTML?

HTML stands for **HyperText Markup Language**.

It is the standard markup language used to create and structure content on webpages.

HTML tells the browser what content exists on a webpage and how that content is organized.

For example, HTML can define:

- Headings
- Paragraphs
- Images
- Links
- Lists
- Tables
- Forms
- Buttons

HTML is the foundation of almost every website.

### Example

```html
<h1>Welcome to My Website</h1>

<p>This is my first webpage.</p>
```

Output:

# Welcome to My Website

This is my first webpage.

The browser reads the HTML and displays the content according to the meaning of its elements.

## 1.2 Why is HTML important?

HTML provides the structure of a webpage.

Without HTML, browsers would not have the structured document that defines the content and organization of a typical website.

For example, consider a recipe webpage:

- A heading represents the recipe name.
- A paragraph describes the recipe.
- An unordered list contains ingredients.
- An ordered list contains cooking instructions.
- An image displays the finished food.
- A link connects the recipe to another page.

HTML organizes all these components.

## 1.3 Is HTML a programming language?

No. HTML is a **markup language**, not a programming language.

A programming language is used to implement logic, calculations, conditions, loops and other computational operations.

HTML primarily describes the structure and meaning of content.

HTML does not independently provide programming logic.

---

# 2. HTML vs CSS vs JavaScript

These three technologies work together to create modern websites.

| Technology | Full Form | Main Responsibility |
|---|---|---|
| HTML | HyperText Markup Language | Structure and content |
| CSS | Cascading Style Sheets | Appearance and styling |
| JavaScript | JavaScript | Behavior and interactivity |

## 2.1 HTML – Structure

HTML defines the content of a webpage.

```html
<h1>My Portfolio</h1>

<p>Welcome to my portfolio website.</p>

<button>Contact Me</button>
```

HTML creates the heading, paragraph and button.

## 2.2 CSS – Styling

CSS controls how HTML elements look.

```css
h1 {
    color: blue;
    font-size: 36px;
}

p {
    color: gray;
}
```

CSS can control:

- Colors
- Fonts
- Backgrounds
- Spacing
- Layouts
- Borders
- Element positioning

## 2.3 JavaScript – Behavior

JavaScript adds functionality and interactivity.

```javascript
const button = document.querySelector("button");

button.addEventListener("click", function () {
    alert("Hello!");
});
```

When the user clicks the button, JavaScript displays a message.

### Easy way to remember

Imagine a house:

- HTML = Structure of the house.
- CSS = Paint, decoration and appearance.
- JavaScript = Electrical systems and interactive features.

All three have different responsibilities but work together.

---

# 3. HTML Elements and Tags

Understanding elements and tags is one of the most important HTML fundamentals.

## 3.1 What is an HTML tag?

A tag is a keyword enclosed in angle brackets.

Example:

```html
<p>
```

This is an opening paragraph tag.

HTML tags tell the browser what kind of element is being used.

## 3.2 What is an HTML element?

An HTML element generally consists of:

1. Opening tag
2. Content
3. Closing tag

Example:

```html
<p>Hello World!</p>
```

Breaking it down:

```html
<p>          <!-- Opening tag -->
Hello World! <!-- Content -->
</p>         <!-- Closing tag -->
```

The complete structure is called an HTML element.

### Difference between tags and elements

| Tag | Element |
|---|---|
| A markup instruction enclosed in angle brackets | The complete HTML structure |
| Example: `<p>` | Example: `<p>Hello</p>` |
| Opens or closes an element | Contains tags and possibly content |

## 3.3 Opening Tags

An opening tag marks the beginning of an element.

Example:

```html
<h1>
```

## 3.4 Closing Tags

A closing tag marks the end of an element.

It contains a forward slash `/` before the tag name.

Example:

```html
</h1>
```

## 3.5 Complete Element Example

```html
<h1>My First Website</h1>
```

- `<h1>` = Opening tag.
- `My First Website` = Content.
- `</h1>` = Closing tag.
- Entire structure = HTML element.

## 3.6 Void Elements

Some HTML elements do not contain content and therefore do not require closing tags.

These are called **void elements**.

Examples:

```html
<br>
<hr>
<img src="image.jpg" alt="A landscape">
<meta charset="UTF-8">
```

Common void elements:

| Element | Purpose |
|---|---|
| `<br>` | Creates a line break |
| `<hr>` | Represents a thematic break |
| `<img>` | Embeds an image |
| `<meta>` | Provides document metadata |
| `<input>` | Creates an input control |
| `<link>` | Links external resources |
| `<area>` | Defines an area inside an image map |
| `<source>` | Specifies media resources |
| `<wbr>` | Suggests a word-break opportunity |
| `<col>` | Defines properties for table columns |
| `<embed>` | Embeds external content |
| `<track>` | Provides text tracks for media |

**Important:** HTML void elements must not have closing tags. You may encounter `<br />` or `<img />` in older examples, but the trailing slash is unnecessary in HTML.

---

# 4. HTML Attributes

## 4.1 What is an attribute?

An HTML attribute provides additional information about an element.

Attributes are written inside the opening tag.

Example:

```html
<a href="https://www.google.com">Google</a>
```

Breaking it down:

- `<a>` = Anchor tag.
- `href` = Attribute name.
- `https://www.google.com` = Attribute value.
- `Google` = Visible link text.

## 4.2 General Attribute Syntax

```html
<tagname attribute="value">Content</tagname>
```

Example:

```html
<img src="cat.jpg" alt="A cat">
```

Here:

- `src` specifies the image location.
- `alt` provides alternative text.

## 4.3 Multiple Attributes

An element can have multiple attributes.

```html
<img
    src="images/cat.jpg"
    alt="A brown cat sitting on a chair"
    width="300"
>
```

Attributes are separated by spaces.

## 4.4 Common HTML Attributes

| Attribute | Purpose |
|---|---|
| `href` | Specifies a link destination |
| `src` | Specifies a resource location |
| `alt` | Provides alternative text for images |
| `id` | Gives an element a unique identifier |
| `class` | Assigns one or more class names |
| `title` | Provides additional advisory information |
| `lang` | Specifies the language |
| `width` | Specifies width |
| `height` | Specifies height |
| `target` | Specifies where to open a linked resource |
| `rel` | Defines the relationship between linked resources |

### Example

```html
<p id="intro" class="description">
    Welcome to my website.
</p>
```

Here:

- `id="intro"` identifies the element.
- `class="description"` assigns it a class.

Note: `id` values should be unique within an HTML document. Multiple elements can share a class.

---

# 5. HTML Boilerplate

## 5.1 What is HTML Boilerplate?

HTML boilerplate is the standard starting structure of an HTML document.

Every normal HTML webpage should begin with this basic structure.

It provides the browser with the necessary document information and establishes the page structure.

## 5.2 Standard HTML Boilerplate

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Webpage</title>
</head>

<body>

    <h1>Hello World!</h1>

</body>

</html>
```

Now let's understand every part.

## 5.3 DOCTYPE Declaration

```html
<!DOCTYPE html>
```

The DOCTYPE declaration tells the browser to interpret the document using modern HTML standards.

For HTML5, the declaration is:

```html
<!DOCTYPE html>
```

Important points:

- It is written at the beginning of the document.
- It is not an HTML element.
- It is not written with a closing tag.
- It helps the browser avoid quirks mode and use standards mode.

## 5.4 HTML Root Element

```html
<html lang="en">
</html>
```

The `<html>` element is the root element of the HTML document.

All other HTML elements are contained within it, except the DOCTYPE declaration.

The `lang` attribute specifies the document's language.

Example:

```html
<html lang="en">
```

Here, `en` represents English.

For a document primarily written in Urdu, the language code would be:

```html
<html lang="ur">
```

## 5.5 Head Element

```html
<head>
    <meta charset="UTF-8">
    <title>My Website</title>
</head>
```

The `<head>` element contains metadata and information needed by the browser and other systems.

It does not contain the normal visible webpage content.

Common elements inside `<head>` include:

- `<meta>`
- `<title>`
- `<link>`
- `<style>`
- `<script>` (with appropriate placement and loading behavior)

## 5.6 Meta Charset

```html
<meta charset="UTF-8">
```

This specifies the character encoding of the document.

UTF-8 supports a wide range of characters and symbols from different languages.

Without a correct character encoding, some characters might display incorrectly.

## 5.7 Meta Viewport

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

This helps browsers display the webpage correctly on different screen sizes.

Breaking it down:

- `name="viewport"` identifies the viewport metadata.
- `width=device-width` sets the viewport width to the device's width.
- `initial-scale=1.0` sets the initial zoom level.

This is especially important for responsive web design.

## 5.8 Title Element

```html
<title>My First Webpage</title>
```

The `<title>` element specifies the webpage title.

It normally appears in:

- Browser tabs.
- Browser bookmarks.
- Search engine results, where appropriate.

It belongs inside `<head>`.

## 5.9 Body Element

```html
<body>
    <h1>Hello World!</h1>
    <p>This is my first webpage.</p>
</body>
```

The `<body>` element contains the webpage's main visible content.

Examples:

- Headings
- Paragraphs
- Images
- Links
- Lists
- Other page content

### Head vs Body

| Head | Body |
|---|---|
| Contains document metadata | Contains webpage content |
| Usually not displayed as page content | Displays content in the browser |
| Contains title and meta information | Contains headings, paragraphs, images, etc. |

## 5.10 Why is the homepage named index.html?

The conventional homepage filename is:

```text
index.html
```

Web servers commonly look for `index.html` as the default document when someone visits a directory or website.

For example:

```text
my-website/
│
├── index.html
├── about.html
└── contact.html
```

The `index.html` file will normally serve as the homepage.

## 5.11 Generating Boilerplate in VS Code

VS Code supports Emmet abbreviations.

Steps:

1. Create a file named `index.html`.
2. Open it in VS Code.
3. Type `!`.
4. Press Enter when the Emmet abbreviation appears.

VS Code will generate the basic HTML boilerplate.

---

# 6. HTML Document Structure

HTML elements can be arranged inside one another to form a document tree.

Example:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>My Website</title>
</head>

<body>

    <h1>Welcome</h1>

    <p>This is a paragraph.</p>

</body>

</html>
```

The hierarchy is:

```text
Document
│
├── DOCTYPE
│
└── html
    │
    ├── head
    │   ├── meta
    │   └── title
    │
    └── body
        ├── h1
        └── p
```

This tree-like structure is called the **DOM (Document Object Model)** when represented as a browser-accessible document structure.

Understanding this hierarchy becomes especially important when working with JavaScript.

---

# 7. Working with Text

Text is one of the most common forms of content on webpages.

HTML provides different elements to organize and give meaning to text.

The most important elements covered in Foundations are:

- `<h1>` through `<h6>`
- `<p>`
- `<strong>`
- `<em>`

---

# 8. HTML Headings

HTML provides six heading levels.

```html
<h1>Main Heading</h1>
<h2>Second-Level Heading</h2>
<h3>Third-Level Heading</h3>
<h4>Fourth-Level Heading</h4>
<h5>Fifth-Level Heading</h5>
<h6>Sixth-Level Heading</h6>
```

## 8.1 Heading Levels

| Tag | Description |
|---|---|
| `<h1>` | Highest-level heading |
| `<h2>` | Second-level heading |
| `<h3>` | Third-level heading |
| `<h4>` | Fourth-level heading |
| `<h5>` | Fifth-level heading |
| `<h6>` | Lowest-level heading |

The heading levels communicate the hierarchy of the content.

Example:

```html
<h1>Web Development</h1>

<h2>Frontend Development</h2>

<h3>HTML</h3>

<h3>CSS</h3>

<h2>Backend Development</h2>

<h3>Node.js</h3>
```

## 8.2 Why are headings important?

Headings:

1. Organize webpage content.
2. Make content easier to understand.
3. Help users navigate information.
4. Provide structure for assistive technologies.
5. Help search engines understand page organization.

**Important:** Do not select a heading level simply because its default font size looks attractive. Choose it according to the document hierarchy. CSS can control appearance.

---

# 9. Paragraphs

The `<p>` element defines a paragraph.

Example:

```html
<p>
    HTML is used to structure webpages.
</p>
```

Multiple paragraphs:

```html
<p>HTML defines webpage structure.</p>

<p>CSS controls webpage appearance.</p>

<p>JavaScript adds interactivity.</p>
```

Each paragraph is a separate element.

## 9.1 Why not just write text directly inside body?

Consider:

```html
<body>
    First paragraph.

    Second paragraph.
</body>
```

HTML source-code line breaks and spaces do not automatically create separate paragraphs.

The browser generally collapses consecutive whitespace when displaying normal HTML text.

Correct approach:

```html
<body>

    <p>First paragraph.</p>

    <p>Second paragraph.</p>

</body>
```

This explicitly communicates the document structure.

---

# 10. Bold and Italic Text

HTML provides elements to emphasize or highlight text.

## 10.1 Strong Element

The `<strong>` element indicates that its content has strong importance, seriousness or urgency.

Example:

```html
<p>
    <strong>Warning:</strong> Save your work before closing.
</p>
```

Browsers generally display strong text in bold.

## 10.2 Emphasis Element

The `<em>` element indicates stress emphasis.

Example:

```html
<p>
    You <em>must</em> complete the assignment.
</p>
```

Browsers generally display emphasized text in italics.

## 10.3 Difference Between Strong and Em

| `<strong>` | `<em>` |
|---|---|
| Indicates strong importance | Indicates stress emphasis |
| Usually appears bold | Usually appears italic |
| Communicates importance | Communicates emphasis |

## 10.4 Bold and Italic Appearance vs Meaning

There are also:

```html
<b>Bold-looking text</b>

<i>Italic-looking text</i>
```

Difference:

- `<b>` draws attention without necessarily indicating importance.
- `<i>` represents text in an alternate voice or mood, or otherwise distinguished from normal prose.
- `<strong>` communicates importance.
- `<em>` communicates stress emphasis.

For ordinary emphasis and importance, use `<em>` and `<strong>` appropriately.

---

# 11. HTML Nesting and Indentation

## 11.1 What is Nesting?

Nesting means placing one HTML element inside another HTML element.

Example:

```html
<p>
    This is a paragraph containing
    <strong>important text</strong>.
</p>
```

Here, `<strong>` is nested inside `<p>`.

## 11.2 Parent and Child Elements

In the example:

```html
<body>
    <p>Hello World!</p>
</body>
```

- `<body>` is the parent element.
- `<p>` is the child element.

The `<p>` element is a descendant of `<body>`.

## 11.3 Sibling Elements

Elements that share the same parent are siblings.

Example:

```html
<body>
    <h1>Welcome</h1>

    <p>First paragraph.</p>

    <p>Second paragraph.</p>
</body>
```

The heading and both paragraphs are siblings.

## 11.4 Proper Nesting

Correct:

```html
<p>
    This is <strong>important</strong> information.
</p>
```

Incorrect:

```html
<p>
    This is <strong>important</p></strong>
```

The second example closes the paragraph before closing the strong element.

HTML elements must be nested according to their permitted content models and proper structural rules.

## 11.5 Indentation

Indentation means adding spaces to show the hierarchy of HTML elements.

Correct:

```html
<body>
    <h1>My Website</h1>

    <div>
        <p>First paragraph.</p>
        <p>Second paragraph.</p>
    </div>
</body>
```

Poorly formatted:

```html
<body>
<h1>My Website</h1>
<div>
<p>First paragraph.</p>
<p>Second paragraph.</p>
</div>
</body>
```

Both may render similarly, but the first is easier to read and maintain.

**Recommended practice:** Use consistent indentation, commonly two or four spaces.

---

# 12. HTML Comments

Comments allow developers to write explanations inside HTML source code.

Comments are not displayed as normal webpage content.

Syntax:

```html
<!-- This is an HTML comment -->
```

Example:

```html
<body>

    <!-- Main heading -->
    <h1>My Website</h1>

    <!-- Introduction section -->
    <p>Welcome to my website.</p>

</body>
```

## 12.1 Why use comments?

- Explain complex code.
- Identify sections.
- Make code easier to understand.
- Temporarily annotate development work.

## 12.2 Important Points

- Comments start with `<!--`.
- Comments end with `-->`.
- Browsers do not display their contents as normal page text.
- Comments are still visible to anyone who inspects the page source.
- Never put passwords, API keys or private information in comments.

---

# 13. HTML Lists

HTML provides different list elements to organize information.

The two basic list types covered in Foundations are:

1. Unordered lists.
2. Ordered lists.

Both use the `<li>` element for individual list items.

---

# 14. Unordered Lists

An unordered list is used when the order of items does not matter.

It is created using:

```html
<ul>
```

Individual items are created using:

```html
<li>
```

## 14.1 Syntax

```html
<ul>
    <li>Apple</li>
    <li>Banana</li>
    <li>Orange</li>
</ul>
```

Output:

- Apple
- Banana
- Orange

## 14.2 When should you use unordered lists?

Examples:

- Shopping lists.
- Ingredients.
- Categories.
- Features.
- Lists of hobbies.

### Example: Shopping List

```html
<h2>Shopping List</h2>

<ul>
    <li>Milk</li>
    <li>Bread</li>
    <li>Eggs</li>
    <li>Rice</li>
</ul>
```

## 14.3 Important Points

- `<ul>` creates an unordered list.
- `<li>` defines an individual list item.
- Items are normally displayed with bullet points.
- The order is not meaningful.

---

# 15. Ordered Lists

An ordered list is used when the sequence of items matters.

It is created using:

```html
<ol>
```

Individual items are created using:

```html
<li>
```

## 15.1 Syntax

```html
<ol>
    <li>Wake up</li>
    <li>Brush your teeth</li>
    <li>Have breakfast</li>
</ol>
```

Output:

1. Wake up
2. Brush your teeth
3. Have breakfast

## 15.2 When should you use ordered lists?

Examples:

- Cooking instructions.
- Tutorials.
- Step-by-step procedures.
- Rankings.
- Sequential processes.

### Example: Recipe Instructions

```html
<h2>Cooking Instructions</h2>

<ol>
    <li>Prepare the ingredients.</li>
    <li>Heat the pan.</li>
    <li>Add the ingredients.</li>
    <li>Cook until ready.</li>
</ol>
```

## 15.3 Ordered List Attributes

The `<ol>` element supports attributes such as:

```html
<ol start="5">
    <li>Fifth item</li>
    <li>Sixth item</li>
</ol>
```

The list starts counting from 5.

You can also use:

```html
<ol reversed>
    <li>Third</li>
    <li>Second</li>
    <li>First</li>
</ol>
```

This reverses the numbering direction.

The `type` attribute can change the numbering style:

```html
<ol type="A">
    <li>First</li>
    <li>Second</li>
</ol>
```

Common values:

- `1` = Numbers
- `A` = Uppercase letters
- `a` = Lowercase letters
- `I` = Uppercase Roman numerals
- `i` = Lowercase Roman numerals

These are additional HTML features beyond the basic Foundations list lesson.

---

# 16. Nested Lists

A nested list is a list placed inside another list item.

Example:

```html
<ul>

    <li>Fruits
        <ul>
            <li>Apple</li>
            <li>Banana</li>
            <li>Orange</li>
        </ul>
    </li>

    <li>Vegetables
        <ul>
            <li>Potato</li>
            <li>Carrot</li>
        </ul>
    </li>

</ul>
```

Output:

- Fruits
  - Apple
  - Banana
  - Orange
- Vegetables
  - Potato
  - Carrot

The nested `<ul>` belongs inside the relevant `<li>`.

You can also nest an ordered list inside an unordered list and vice versa.

Example:

```html
<ul>
    <li>Web Development
        <ol>
            <li>Learn HTML</li>
            <li>Learn CSS</li>
            <li>Learn JavaScript</li>
        </ol>
    </li>
</ul>
```

---

# 17. HTML Links

Links are one of the most important features of HTML.

They connect webpages and allow users to navigate between different resources.

The HTML element used to create a link is:

```html
<a>
```

It is called the **anchor element**.

## 17.1 Basic Link Syntax

```html
<a href="https://www.google.com">Visit Google</a>
```

Breaking it down:

- `<a>` = Anchor element.
- `href` = Hypertext Reference attribute.
- `https://www.google.com` = Destination.
- `Visit Google` = Clickable text.

## 17.2 What is href?

The `href` attribute specifies the destination of a hyperlink.

Without an appropriate `href`, an anchor element does not provide a normal navigational link.

Example:

```html
<a href="https://www.theodinproject.com/">
    The Odin Project
</a>
```

## 17.3 External Links

External links navigate to other websites.

Example:

```html
<a href="https://developer.mozilla.org/">
    MDN Web Docs
</a>
```

## 17.4 Internal Links

Internal links connect pages within the same website.

Example directory:

```text
website/
│
├── index.html
├── about.html
└── contact.html
```

From `index.html`, create a link to `about.html`:

```html
<a href="about.html">About Us</a>
```

From `about.html`, link back to the homepage:

```html
<a href="index.html">Home</a>
```

## 17.5 Open a Link in a New Tab

You can use the `target` attribute:

```html
<a
    href="https://www.google.com"
    target="_blank"
    rel="noopener"
>
    Open Google
</a>
```

- `target="_blank"` generally opens the destination in a new tab.
- `rel="noopener"` prevents the opened page from accessing the original page through `window.opener`.

This is useful additional knowledge for working with external links.

---

# 18. Absolute and Relative Links

Understanding the difference between absolute and relative paths is extremely important.

## 18.1 Absolute URL

An absolute URL contains the complete web address of a resource.

Example:

```html
<a href="https://www.theodinproject.com/">
    The Odin Project
</a>
```

It includes:

- Protocol: `https://`
- Domain: `www.theodinproject.com`
- Optional path: `/`

Absolute URLs are commonly used for external websites.

## 18.2 Relative URL

A relative URL points to a resource based on the location of the current document or the site's configured base URL.

Example:

```html
<a href="about.html">About</a>
```

Here, the browser looks for `about.html` relative to the current document's location.

Relative paths are commonly used for pages and resources within your own website.

## 18.3 Same Directory

Directory structure:

```text
website/
│
├── index.html
└── about.html
```

Link:

```html
<a href="about.html">About</a>
```

Both files are in the same directory.

## 18.4 Child Directory

Directory structure:

```text
website/
│
├── index.html
│
└── pages/
    └── about.html
```

Link:

```html
<a href="pages/about.html">About</a>
```

The `pages/` directory is inside the current directory.

## 18.5 Parent Directory

Directory structure:

```text
website/
│
├── index.html
│
└── pages/
    └── about.html
```

Inside `about.html`, link to the homepage:

```html
<a href="../index.html">Home</a>
```

The `../` notation moves one directory level upward.

## 18.6 Important Path Symbols

| Symbol | Meaning |
|---|---|
| `./` | Current directory |
| `../` | Parent directory |
| `/` | Path separator or, in URL paths, a root-relative path marker |

### Example

```html
<a href="./about.html">About</a>
```

This refers to `about.html` in the current directory.

```html
<a href="../index.html">Home</a>
```

This refers to `index.html` in the parent directory.

---

# 19. HTML Images

HTML allows developers to display images using the `<img>` element.

It is a void element.

## 19.1 Basic Image Syntax

```html
<img src="cat.jpg" alt="A cat">
```

Here:

- `<img>` = Image element.
- `src` = Image source.
- `alt` = Alternative text.

## 19.2 Why is src important?

The `src` attribute specifies the location of the image file.

Example:

```html
<img src="images/dog.jpg" alt="A dog">
```

The browser looks for `dog.jpg` inside the `images` directory relative to the HTML document.

## 19.3 Why is alt important?

The `alt` attribute provides alternative text describing an image.

It is important for:

1. Accessibility.
2. Screen readers.
3. Situations where an image cannot load.
4. Understanding the purpose or content of an image.

Example:

```html
<img
    src="images/burger.jpg"
    alt="A cheeseburger with lettuce and tomato"
>
```

If the image cannot be displayed, the alternative text can help communicate what the image represents.

For purely decorative images, an empty alternative text is generally appropriate:

```html
<img src="decoration.png" alt="">
```

## 19.4 Image Using a Relative Path

Directory:

```text
website/
│
├── index.html
│
└── images/
    ├── burger.jpg
    └── pizza.jpg
```

HTML:

```html
<img src="images/burger.jpg" alt="A burger">

<img src="images/pizza.jpg" alt="A pizza">
```

## 19.5 Image Using an Absolute URL

You can also load an image from an external website:

```html
<img
    src="https://example.com/image.jpg"
    alt="Example image"
>
```

The image must be publicly accessible for the browser to load it.

## 19.6 Image Dimensions

You can specify image dimensions:

```html
<img
    src="burger.jpg"
    alt="A burger"
    width="400"
    height="300"
>
```

Specifying dimensions can help the browser reserve space for the image before it loads.

CSS is generally preferred for more flexible image sizing and responsive layouts.

---

# 20. File Paths

File paths tell the browser where to find files such as:

- HTML pages.
- Images.
- CSS files.
- JavaScript files.

Example:

```text
my-website/
│
├── index.html
│
├── about.html
│
└── images/
    ├── logo.png
    └── profile.jpg
```

Inside `index.html`:

```html
<img src="images/logo.png" alt="Website logo">
```

The browser follows this path:

1. Start from the directory containing `index.html`.
2. Find the `images` directory.
3. Find `logo.png`.
4. Load the image.

## 20.1 Relative Path Examples

| Path | Meaning |
|---|---|
| `image.jpg` | File in the current directory |
| `images/image.jpg` | File inside images directory |
| `../image.jpg` | File in the parent directory |
| `./image.jpg` | File in the current directory |

## 20.2 Common Path Errors

Incorrect:

```html
<img src="image/burger.jpg" alt="Burger">
```

But the actual directory is named `images`.

Correct:

```html
<img src="images/burger.jpg" alt="Burger">
```

Other common problems:

- Incorrect filename.
- Incorrect file extension.
- Wrong directory name.
- Incorrect capitalization on case-sensitive servers.
- Incorrect number of `../` segments.

---

# 21. Semantic HTML – Additional Knowledge

Semantic HTML means using HTML elements according to the meaning and purpose of their content.

For example:

```html
<h1>About Us</h1>

<p>We build websites.</p>
```

This is more meaningful than using generic elements for every piece of content.

## 21.1 Common Semantic Elements

| Element | Purpose |
|---|---|
| `<header>` | Introductory content for a page or section |
| `<nav>` | Navigation links |
| `<main>` | Main content of the document |
| `<section>` | Thematic grouping of content |
| `<article>` | Self-contained composition |
| `<aside>` | Complementary content |
| `<footer>` | Footer information |

Example:

```html
<body>

    <header>
        <h1>My Website</h1>
    </header>

    <nav>
        <a href="index.html">Home</a>
        <a href="about.html">About</a>
    </nav>

    <main>
        <section>
            <h2>Introduction</h2>
            <p>Welcome to my website.</p>
        </section>
    </main>

    <footer>
        <p>Copyright 2026</p>
    </footer>

</body>
```

Semantic HTML improves document structure, accessibility and maintainability.

These elements are supplementary knowledge; the initial Foundations HTML lessons introduce only the basics of semantic markup.

---

# 22. HTML Validation and Common Errors

HTML validation checks whether your HTML follows the relevant HTML syntax and conformance rules.

An HTML validator can identify:

- Missing required attributes.
- Incorrect nesting.
- Invalid elements.
- Incorrect attributes.
- Unclosed tags.
- Other markup errors.

## 22.1 W3C HTML Validator

The W3C HTML Validator is a useful tool for checking HTML documents.

Website:

https://validator.w3.org/

You can validate HTML by:

- Providing a webpage URL.
- Uploading an HTML file.
- Pasting HTML code.

## 22.2 Common HTML Errors

### Error 1: Missing Closing Tag

Incorrect:

```html
<p>Hello World!
```

Correct:

```html
<p>Hello World!</p>
```

### Error 2: Incorrect Nesting

Incorrect:

```html
<p>
    <strong>Hello</p>
</strong>
```

Correct:

```html
<p>
    <strong>Hello</strong>
</p>
```

### Error 3: Missing Attribute Value

Incorrect:

```html
<a href>Google</a>
```

Correct:

```html
<a href="https://www.google.com">Google</a>
```

### Error 4: Missing Image Alternative Text

Incorrect:

```html
<img src="cat.jpg">
```

Better:

```html
<img src="cat.jpg" alt="A cat">
```

### Error 5: Incorrect File Path

Incorrect:

```html
<img src="burger.jpg" alt="Burger">
```

If the image is actually in the `images` directory, use:

```html
<img src="images/burger.jpg" alt="Burger">
```

### Error 6: Incorrect HTML Boilerplate

Incorrect:

```html
<html>
<body>
    <h1>Hello</h1>
</body>
</html>
```

This may render, but it lacks the recommended modern document structure.

Better:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Website</title>
</head>

<body>
    <h1>Hello</h1>
</body>
</html>
```

---

# 23. The Odin Project: Recipes Project

The Recipes project is the practical project used to apply the HTML knowledge learned throughout the Foundations HTML lessons.

## 23.1 Project Objective

Create a basic recipe website containing:

- A main homepage.
- Links to individual recipe pages.
- Recipe descriptions.
- Ingredients.
- Cooking instructions.
- Images.

The purpose is to practise HTML structure, text, lists, links and images.

## 23.2 Recommended Directory Structure

```text
odin-recipes/
│
├── index.html
│
├── recipes/
│   ├── burger.html
│   ├── pizza.html
│   └── pasta.html
│
└── images/
    ├── burger.jpg
    ├── pizza.jpg
    └── pasta.jpg
```

## 23.3 Homepage Example

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Odin Recipes</title>
</head>

<body>

    <h1>Odin Recipes</h1>

    <ul>
        <li>
            <a href="recipes/burger.html">Burger Recipe</a>
        </li>

        <li>
            <a href="recipes/pizza.html">Pizza Recipe</a>
        </li>

        <li>
            <a href="recipes/pasta.html">Pasta Recipe</a>
        </li>
    </ul>

</body>

</html>
```

## 23.4 Individual Recipe Page Example

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Burger Recipe</title>
</head>

<body>

    <h1>Homemade Burger</h1>

    <img
        src="../images/burger.jpg"
        alt="Homemade burger"
    >

    <h2>Description</h2>

    <p>
        A homemade burger prepared with a bun,
        vegetables, cheese and a burger patty.
    </p>

    <h2>Ingredients</h2>

    <ul>
        <li>Burger bun</li>
        <li>Cheese</li>
        <li>Lettuce</li>
        <li>Tomato</li>
        <li>Burger patty</li>
    </ul>

    <h2>Steps</h2>

    <ol>
        <li>Prepare the ingredients.</li>
        <li>Prepare the burger patty.</li>
        <li>Arrange the ingredients inside the bun.</li>
        <li>Serve the burger.</li>
    </ol>

    <a href="../index.html">Back to Homepage</a>

</body>

</html>
```

## 23.5 HTML Concepts Used in the Project

| HTML Concept | Where It Is Used |
|---|---|
| Boilerplate | Every HTML page |
| Headings | Recipe names and sections |
| Paragraphs | Recipe descriptions |
| Strong/Emphasis | Important text, where appropriate |
| Unordered Lists | Ingredients |
| Ordered Lists | Cooking instructions |
| Anchor Elements | Navigation between pages |
| Images | Recipe pictures |
| Relative Paths | Connecting pages and images |

## 23.6 What Did I Learn?

By completing the Recipes project, I practised:

- Creating multiple HTML pages.
- Structuring content using headings.
- Writing paragraphs.
- Creating ordered and unordered lists.
- Linking webpages.
- Adding images.
- Organizing project directories.
- Understanding relative file paths.
- Creating a basic website without CSS.

---

# 24. Important HTML Tags Reference

This section is useful for quick revision.

| Tag | Name | Purpose |
|---|---|---|
| `<!DOCTYPE html>` | Doctype | Declares HTML document type |
| `<html>` | HTML | Root element |
| `<head>` | Head | Document metadata |
| `<body>` | Body | Visible page content |
| `<title>` | Title | Browser tab title |
| `<meta>` | Meta | Document metadata |
| `<h1>` | Heading 1 | Main-level heading |
| `<h2>` | Heading 2 | Second-level heading |
| `<h3>` | Heading 3 | Third-level heading |
| `<h4>` | Heading 4 | Fourth-level heading |
| `<h5>` | Heading 5 | Fifth-level heading |
| `<h6>` | Heading 6 | Sixth-level heading |
| `<p>` | Paragraph | Paragraph text |
| `<strong>` | Strong | Important text |
| `<em>` | Emphasis | Stressed text |
| `<b>` | Bold | Stylistically distinguished text |
| `<i>` | Italic | Alternate voice or mood |
| `<br>` | Break | Line break |
| `<hr>` | Horizontal Rule | Thematic break |
| `<ul>` | Unordered List | Bulleted list |
| `<ol>` | Ordered List | Numbered list |
| `<li>` | List Item | Individual list entry |
| `<a>` | Anchor | Hyperlink |
| `<img>` | Image | Embeds an image |
| `<div>` | Division | Generic block container |
| `<span>` | Span | Generic inline container |
| `<header>` | Header | Introductory content |
| `<nav>` | Navigation | Navigation section |
| `<main>` | Main | Main page content |
| `<section>` | Section | Thematic grouping |
| `<article>` | Article | Self-contained content |
| `<footer>` | Footer | Footer information |

---

# 25. Common Mistakes to Avoid

1. Confusing HTML tags with HTML elements.
2. Forgetting closing tags for elements that require them.
3. Incorrectly nesting HTML elements.
4. Using headings simply to make text larger.
5. Using paragraphs instead of lists when content is better represented as a list.
6. Confusing `<ol>` and `<ul>`.
7. Forgetting the `href` attribute in links.
8. Forgetting the `src` attribute in images.
9. Forgetting alternative text for meaningful images.
10. Using incorrect relative paths.
11. Placing visible webpage content inside `<head>`.
12. Forgetting `<!DOCTYPE html>`.
13. Forgetting the `<title>` element.
14. Using inconsistent indentation.
15. Assuming HTML whitespace in the source always appears the same in the browser.

---

# 26. Exam Preparation Questions

Try answering these questions without looking at the notes.

## Part A: Basic Concepts

**Q1.** What does HTML stand for?

**Q2.** What is the primary purpose of HTML?

**Q3.** Is HTML a programming language? Explain.

**Q4.** What is the difference between HTML, CSS and JavaScript?

**Q5.** What is an HTML tag?

**Q6.** What is an HTML element?

**Q7.** Explain the difference between an opening tag and a closing tag.

**Q8.** What are void elements? Give five examples.

**Q9.** What are HTML attributes?

**Q10.** What is the purpose of the `href` attribute?

## Part B: HTML Boilerplate

**Q11.** What is HTML boilerplate?

**Q12.** What is the purpose of `<!DOCTYPE html>`?

**Q13.** What is the root element of an HTML document?

**Q14.** What is the purpose of the `<head>` element?

**Q15.** What is the purpose of the `<body>` element?

**Q16.** What does `<meta charset="UTF-8">` do?

**Q17.** What is the purpose of the `<title>` element?

**Q18.** Why do we commonly name a homepage `index.html`?

**Q19.** What is the purpose of the `lang` attribute?

**Q20.** What does the viewport meta tag do?

## Part C: Text and Lists

**Q21.** How many heading levels are available in HTML?

**Q22.** What is the difference between `<h1>` and `<h6>`?

**Q23.** Which element creates a paragraph?

**Q24.** What is the difference between `<strong>` and `<em>`?

**Q25.** What is nesting in HTML?

**Q26.** What is the difference between parent and child elements?

**Q27.** What are sibling elements?

**Q28.** What is an HTML comment?

**Q29.** Which element creates an unordered list?

**Q30.** Which element creates an ordered list?

**Q31.** What is the purpose of `<li>`?

**Q32.** When should you use an ordered list instead of an unordered list?

## Part D: Links and Images

**Q33.** What is an anchor element?

**Q34.** What does `href` stand for?

**Q35.** What is the difference between absolute and relative URLs?

**Q36.** What does `../` mean in a file path?

**Q37.** Which HTML element is used to display an image?

**Q38.** What is the purpose of the `src` attribute?

**Q39.** What is the purpose of the `alt` attribute?

**Q40.** Why are relative paths important when building websites?

## Part E: Practical Questions

**Q41.** Write a complete HTML boilerplate.

**Q42.** Create an HTML page containing one heading and two paragraphs.

**Q43.** Create an unordered list of five programming languages.

**Q44.** Create an ordered list of five steps for completing a project.

**Q45.** Create a hyperlink to The Odin Project.

**Q46.** Display an image named `profile.jpg` stored inside an `images` folder.

**Q47.** Create a nested list containing programming languages and their frameworks.

**Q48.** Explain how you would link `about.html` from `index.html` when both files are in the same directory.

**Q49.** Explain how to navigate from `pages/about.html` to `index.html` in its parent directory.

**Q50.** Describe the structure and functionality of the Odin Recipes project.

---

# 27. Practical Exercises

Complete these exercises to test your understanding.

## Exercise 1: Basic Webpage

Create an HTML page containing:

- A complete HTML boilerplate.
- A title.
- One main heading.
- Three paragraphs.
- One strong element.
- One emphasis element.

## Exercise 2: Shopping List

Create an unordered list containing:

- Five food items.
- Three beverages.
- Four household items.

## Exercise 3: Daily Routine

Create an ordered list describing your daily routine.

Use at least five list items.

## Exercise 4: Nested List

Create a nested list:

- Frontend Development
  - HTML
  - CSS
  - JavaScript
- Backend Development
  - Node.js
  - Express
  - Databases

## Exercise 5: Links

Create a webpage with links to:

- The Odin Project.
- MDN Web Docs.
- GitHub.

## Exercise 6: Images

Create a webpage displaying three images.

Requirements:

- Use the `<img>` element.
- Use relative paths.
- Include meaningful alternative text.

## Exercise 7: Mini Website

Create a three-page website:

```text
mini-website/
│
├── index.html
├── about.html
└── contact.html
```

Requirements:

- Add navigation links between pages.
- Use headings and paragraphs.
- Add at least one image.
- Use a complete HTML boilerplate on every page.

---

# 28. Quick Revision Sheet

| Concept | Remember |
|---|---|
| HTML | Structures webpage content |
| CSS | Styles webpage content |
| JavaScript | Adds functionality |
| Tag | Markup enclosed in angle brackets |
| Element | Complete HTML structure |
| Attribute | Additional element information |
| Void Element | Element without a closing tag |
| DOCTYPE | Declares modern HTML document type |
| HTML Root | `<html>` |
| Metadata | `<head>` |
| Visible Content | `<body>` |
| Browser Title | `<title>` |
| Character Encoding | `<meta charset="UTF-8">` |
| Heading | `<h1>` to `<h6>` |
| Paragraph | `<p>` |
| Strong Importance | `<strong>` |
| Stress Emphasis | `<em>` |
| Comment | `<!-- comment -->` |
| Unordered List | `<ul>` |
| Ordered List | `<ol>` |
| List Item | `<li>` |
| Hyperlink | `<a>` |
| Link Destination | `href` |
| Image | `<img>` |
| Image Location | `src` |
| Alternative Text | `alt` |
| Current Directory | `./` |
| Parent Directory | `../` |

---

# 29. Final HTML Checklist

Before considering your HTML fundamentals complete, make sure you can:

- [ ] Explain what HTML is.
- [ ] Differentiate HTML, CSS and JavaScript.
- [ ] Explain tags and elements.
- [ ] Identify void elements.
- [ ] Explain HTML attributes.
- [ ] Write HTML boilerplate independently.
- [ ] Explain the purpose of head and body.
- [ ] Use headings and paragraphs correctly.
- [ ] Understand strong and emphasis elements.
- [ ] Nest HTML elements correctly.
- [ ] Write HTML comments.
- [ ] Create unordered and ordered lists.
- [ ] Create nested lists.
- [ ] Create internal and external links.
- [ ] Differentiate absolute and relative URLs.
- [ ] Display images using the img element.
- [ ] Use image alternative text.
- [ ] Understand relative file paths.
- [ ] Build a multi-page HTML website.
- [ ] Validate HTML code.

---

## Final Thoughts

HTML is the foundation upon which the rest of web development is built.

Do not rush through these fundamentals. Understanding document structure, elements, attributes, nesting, lists, links and images will make CSS and JavaScript considerably easier to learn.

**Learning sequence:**

HTML Structure → HTML Elements → Text → Lists → Links → Images → Practical Projects

**Learn the structure first. Style it later. Make it interactive after that.**

---

## Official Learning References

1. [The Odin Project – Foundations](https://www.theodinproject.com/paths/foundations/courses/foundations)
2. [Introduction to HTML and CSS](https://www.theodinproject.com/lessons/foundations-introduction-to-html-and-css)
3. [Elements and Tags](https://www.theodinproject.com/lessons/foundations-elements-and-tags)
4. [HTML Boilerplate](https://www.theodinproject.com/lessons/foundations-html-boilerplate)
5. [Working with Text](https://www.theodinproject.com/lessons/foundations-working-with-text)
6. [Lists](https://www.theodinproject.com/lessons/foundations-lists)
7. [Links and Images](https://www.theodinproject.com/lessons/foundations-links-and-images)
8. [Project: Recipes](https://www.theodinproject.com/lessons/foundations-recipes)
9. [MDN HTML Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML)

**Document:** HTML Foundations Study Notes  
**Repository:** The Odin Project – Web Dev Learning  
**Directory:** `Foundations/04-HTML/notes.md`