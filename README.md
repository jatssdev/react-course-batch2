# 📚 **Session 1 - HTML (HyperText Markup Language)**

## 🎯 **Session Objectives:**
By the end of this session, students will be able to:
- Understand what HTML is and its significance in web development.
- Create a basic HTML document structure.
- Use essential HTML tags to build a simple web page.
- Understand and implement HTML tables.
- Differentiate between semantic and non-semantic elements.
- Recognize singular and paired tags in HTML.

---

## 📝 **Topics Covered:**

### 1. **Introduction to HTML**
- **What is HTML?**  
  HyperText Markup Language (HTML) is the standard markup language for creating web pages.

- **Why is HTML important?**  
  It provides the structure of a webpage, allowing browsers to display content correctly.


- **Difference between HTML, CSS, and JavaScript:**  
  - HTML: Structure  
  - CSS: Styling  
  - JavaScript: Interactivity  

---

### 2. **HTML Document Structure**
- Basic HTML Template:
  ```html
  <!DOCTYPE html>
  <html lang="en">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>My First Webpage</title>
  </head>
  <body>
      <h1>Hello, World!</h1>
  </body>
  </html>
  ```
- Explanation of:
  - `<!DOCTYPE html>`: Declares document type and version of HTML.
  - `<html>`: Root element of the document.
  - `<head>`: Contains metadata, title, and links to styles/scripts.
  - `<title>`: Displays title on browser tab.
  - `<body>`: Contains all visible content.

---

### 3. **HTML Text Formatting Tags**
- Headings: `<h1>` to `<h6>`  
- Paragraphs: `<p>`  
- Bold Text: `<b>` and `<strong>` (semantic emphasis)  
- Italics: `<i>` and `<em>` (semantic emphasis)  
- Line Break: `<br>`  
- Horizontal Rule: `<hr>`  

Example:
```html
<h2>This is a heading</h2>
<p>This is a paragraph.</p>
<strong>This text is important.</strong>
```

---

### 4. **Lists in HTML**
- **Ordered List** (`<ol>`)  
- **Unordered List** (`<ul>`)  
- **Definition List** (`<dl>`, `<dt>`, `<dd>`)  

Example:
```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

---

### 5. **Links and Anchors**
- Basic Links: `<a href="URL">Link Text</a>`  
- Open in New Tab: `target="_blank"`  
- Page Anchors for internal navigation.

Example:
```html
<a href="https://www.jatssdev.com" target="_blank">Visit Jatssdev Technologies</a>
```

---

### 6. **Images in HTML**
- Syntax: `<img src="image.jpg" alt="Description" width="300">`  
- Importance of the `alt` attribute for accessibility.

Example:
```html
<img src="profile.jpg" alt="Profile Picture" width="200">
```

---

### 7. **HTML Tables**
- Basic Table Structure:
  ```html
  <table border="1">
      <tr>
          <th>Name</th>
          <th>Age</th>
          <th>Course</th>
      </tr>
      <tr>
          <td>Raghav</td>
          <td>25</td>
          <td>MERN Stack</td>
      </tr>
      <tr>
          <td>Mahi</td>
          <td>23</td>
          <td>React Native</td>
      </tr>
  </table>
  ```
- Tags Explained:
  - `<table>`: Creates a table.
  - `<tr>`: Table row.
  - `<th>`: Table header (bold and centered by default).
  - `<td>`: Table data cell.

---

### 8. **Semantic vs Non-Semantic Elements**
- **Semantic Elements:** Clearly describe their meaning.
  - Examples: `<header>`, `<footer>`, `<article>`, `<section>`, `<nav>`, `<main>`, `<aside>`

- **Non-Semantic Elements:** Don’t provide clear meaning.
  - Examples: `<div>`, `<span>`

Example:
```html
<header>
    <h1>Welcome to Jatssdev Technologies</h1>
</header>
<section>
    <p>Learn with the best mentors and courses.</p>
</section>
<div>This is a non-semantic container.</div>
```

---

### 9. **Singular (Void) vs Paired Tags**
- **Singular Tags (Void Elements):** Don’t require a closing tag.
  - Examples: `<br>`, `<hr>`, `<img>`, `<input>`, `<meta>`, `<link>`

- **Paired Tags:** Have an opening and closing tag.
  - Examples: `<p></p>`, `<div></div>`, `<h1></h1>`, `<a></a>`

Example:
```html
<p>This is a paired tag example.</p>
<img src="logo.png" alt="Logo"> <!-- Singular tag -->
```

---

### 10. **HTML Comments**
- Syntax:
  ```html
  <!-- This is a comment -->
  ```
- Used for code explanations and reminders.

---

## 🧩 **Hands-on Activity: Build Your First Web Page**
Students will create a **Personal Portfolio Page** including:
✅ Name as a heading  
✅ A short bio in paragraphs  
✅ An unordered list of hobbies  
✅ A table with education details  
✅ A profile picture using `<img>`  
✅ Links to their favorite website  

---

## 🏠 **Homework:**
✅ Create a webpage with:  
- Two headings  
- Three paragraphs about your favorite hobby  
- An unordered list of your top 5 favorite foods  
- A table showing your weekly schedule  
- An image related to your hobby  

---

## 🚀 **Bonus Challenge:**
Create a simple webpage with:
- A **header** and **footer** section  
- A **navigation bar** using semantic elements  
- A table showcasing **course offerings** at Jatssdev Technologies  
- Links that navigate to different sections of the same page  

---
---
---
---
# 📚 **Session 2 - Advanced HTML Concepts**

## 🎯 **Session Objectives:**
By the end of this session, students will be able to:
- Create and manage HTML forms with various input types.
- Embed multimedia content like videos, audio, and external websites.
- Design responsive tables with advanced features.
- Optimize web pages for SEO using meta tags.
- Handle internationalization and character encoding in HTML.
- Understand deprecated and obsolete tags in modern web development.
- Use custom data attributes to store additional data.

---

## 📝 **Topics Covered:**

### 1. **HTML Forms and Input Types**
Forms are essential for collecting user data. This section covers how to create and use them effectively.

#### ✅ Basic Form Structure:
```html
<form action="/submit" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>

    <label for="dob">Date of Birth:</label>
    <input type="date" id="dob" name="dob">

    <label for="gender">Gender:</label>
    <select id="gender" name="gender">
        <option value="male">Male</option>
        <option value="female">Female</option>
        <option value="other">Other</option>
    </select>

    <button type="submit">Submit</button>
</form>
```

#### 🛠️ **Important Form Attributes:**
- `action`: URL where the form data is sent.
- `method`: `GET` or `POST` (data submission type).
- `name`: Identifies form elements.
- `placeholder`, `required`, `disabled`: Enhances user interaction.

#### 🎯 **Advanced Input Types:**
- `<input type="tel">` - Phone numbers  
- `<input type="range">` - Slider controls  
- `<input type="color">` - Color picker  
- `<input type="file">` - File uploads  

Example of File Upload:
```html
<input type="file" name="resume" accept=".pdf,.docx">
```

---

### 2. **Multimedia Elements**
Enhance user experience by adding videos, audio, and external content.

#### 🎥 **Embedding Videos:**
```html
<video width="400" controls>
    <source src="sample-video.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```
- `controls`: Adds play, pause, and volume buttons.
- `autoplay`, `loop`, `muted`: Control playback behavior.

#### 🎧 **Embedding Audio:**
```html
<audio controls>
    <source src="sample-audio.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>
```

#### 🌍 **Using `<iframe>` for External Content:**
```html
<iframe src="https://www.jatssdev.com" width="600" height="400" title="Jatssdev Website"></iframe>
```
- Use for embedding Google Maps, YouTube videos, or other web pages.

---

### 3. **Advanced Tables and Responsive Design**
Tables can organize data effectively. Learn how to make them more dynamic.

#### 📊 **Table with `colspan` and `rowspan`:**
```html
<table border="1">
    <tr>
        <th rowspan="2">Name</th>
        <th colspan="2">Contact Info</th>
    </tr>
    <tr>
        <th>Email</th>
        <th>Phone</th>
    </tr>
    <tr>
        <td>Raghav</td>
        <td>raghav@example.com</td>
        <td>+91 9876543210</td>
    </tr>
</table>
```

#### 📱 **Making Tables Responsive:**
```html
<div style="overflow-x:auto;">
    <table border="1">
        <tr>
            <th>Course</th>
            <th>Duration</th>
            <th>Price</th>
        </tr>
        <tr>
            <td>MERN Stack</td>
            <td>3 months</td>
            <td>₹20,000</td>
        </tr>
    </table>
</div>
```
- Wrapping tables in a scrollable container improves mobile viewing.

---

### 4. **Meta Tags and SEO Basics**
Meta tags help search engines understand your page.

#### 📄 **Common Meta Tags:**
```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Learn web development at Jatssdev Technologies.">
    <meta name="keywords" content="HTML, CSS, Web Development, Jatssdev">
    <title>Jatssdev Courses</title>
</head>
```
- `description`: Appears in search engine results.
- `viewport`: Essential for responsive design.
- `keywords`: (Less significant now but still useful for context.)

---

### 5. **Internationalization and Character Encoding**
Make your website accessible globally.

#### 🌐 **Setting Language:**
```html
<html lang="en">
<body>
    <p>Hello, World!</p>
</body>
</html>
```
- Use appropriate `lang` attributes (`en`, `fr`, `es`, `hi`, etc.).

#### 🔑 **Character Encoding:**
```html
<meta charset="UTF-8">
```
- Ensures special characters display correctly.
- Avoid issues with multilingual content.

---

### 6. **Deprecated and Obsolete Tags**
Stay updated to avoid using outdated tags.

#### 🚫 **Examples of Deprecated Tags:**
- `<center>`: Use CSS `text-align` instead.
- `<font>`: Use CSS for text styling.
- `<marquee>`: Not supported in modern browsers.

#### ✅ **Modern Alternatives:**
```html
<p style="text-align: center;">Centered Text</p>
```

---

### 7. **Custom Data Attributes and Microdata**
Store additional data within HTML elements.

#### 🗂️ **Using `data-*` Attributes:**
```html
<button data-course="MERN Stack" data-price="20000">Enroll Now</button>
```
- Useful for JavaScript-based dynamic functionality.
- Accessed using JS: 
```javascript
const button = document.querySelector('button');
console.log(button.dataset.course); // Output: MERN Stack
```

---

## 🧩 **Hands-on Activity:**
✅ Create a **Course Enrollment Form** with various input types.  
✅ Embed a **YouTube video** of your favorite tutorial.  
✅ Build a **responsive table** showcasing available courses and prices.  
✅ Add **meta tags** to your page for SEO optimization.  
✅ Create a button using **data attributes** to display course info via alert.

---

## 🏠 **Homework:**
✅ Build a **portfolio page** that includes:  
- Personal info form  
- Embedded resume video/audio  
- Table of skills and experience  
- Proper meta tags for SEO  
- Use of at least one `data-*` attribute  

---

## 🚀 **Bonus Challenge:**
Create a **Course Landing Page** with:  
- Header and footer  
- Responsive tables for pricing plans  
- Embedded promotional video  
- Meta tags for search engine optimization  
- Use custom data attributes to show course details on button clicks  

