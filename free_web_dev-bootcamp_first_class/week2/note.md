# Week 2-3: HTML Deep Dive

## Topics Covered

### 1. Semantic HTML

Semantic HTML elements clearly define the purpose of the content they contain. Using them improves readability, SEO, and accessibility.

* **`<header>`**: Represents the introductory section of a page or a section, often containing navigation or branding.

  ```html
  <header>
      <h1>Website Title</h1>
      <nav>
          <a href="#">Home</a>
          <a href="#">About</a>
      </nav>
  </header>
  ```

* **`<section>`**: Groups related content under a common theme or heading.

  ```html
  <section>
      <h2>About Us</h2>
      <p>We provide resources for web developers.</p>
  </section>
  ```

* **`<article>`**: Represents a self-contained piece of content, like a blog post or news article.

  ```html
  <article>
      <h2>Blog Post Title</h2>
      <p>This is the content of the article.</p>
  </article>
  ```

### 2. Forms

Forms allow user input and data submission.

* **Basic form structure:**

  ```html
  <form action="/submit" method="POST">
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required>
      <button type="submit">Submit</button>
  </form>
  ```

* **Other input types:** `email`, `password`, `checkbox`, `radio`, `number`, `date`.

### 3. Tables

Used to display structured tabular data.

```html
<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Age</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Alice</td>
            <td>25</td>
        </tr>
    </tbody>
</table>
```

### 4. Multimedia

Embedding audio and video enhances user experience.

* **Video:**

  ```html
  <video controls width="320">
      <source src="movie.mp4" type="video/mp4">
      Your browser does not support the video tag.
  </video>
  ```

* **Audio:**

  ```html
  <audio controls>
      <source src="audio.mp3" type="audio/mpeg">
      Your browser does not support the audio element.
  </audio>
  ```

### 5. Accessibility Basics

Ensuring your site is accessible to all users, including those using assistive technologies.

* **Alt text for images:**

  ```html
  <img src="logo.png" alt="Company Logo">
  ```
* **ARIA labels:** Add roles and labels to improve screen reader interpretation.

  ```html
  <button aria-label="Close menu">X</button>
  ```



**Tips:**

* Keep your design minimal and clean.
* Focus on correct HTML structure before styling.
* Test your site with a screen reader to ensure accessibility.
