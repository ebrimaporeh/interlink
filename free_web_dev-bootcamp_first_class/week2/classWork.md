# Week 2-3 HTML Deep Dive - Classwork

## Objective

Practice semantic HTML, forms, tables, multimedia, and accessibility basics through small exercises to reinforce learning from the lecture.

---

## Part 1: Semantic HTML

**Task:** Create a small webpage section using semantic HTML.

1. Create a `<header>` with a site title and navigation links.
2. Add a `<section>` describing your favorite hobby.
3. Add an `<article>` representing a small blog post or news item.
4. Include a `<footer>` with your contact information.

> Bonus: Use `<h1>`-`<h3>` appropriately for headings.

```html
<!-- Example structure -->
<header>
  <h1>My Site</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
  </nav>
</header>
<section>
  <h2>My Hobby</h2>
  <p>Describe your hobby here.</p>
</section>
<article>
  <h2>Blog Post</h2>
  <p>Content of the article.</p>
</article>
<footer>
  <p>Contact: example@example.com</p>
</footer>
```

---

## Part 2: Forms

**Task:** Build a simple registration form.

**Requirements:**

1. Include inputs for name, email, password, and a checkbox for agreeing to terms.
2. Add a submit button.
3. Use `<label>`s correctly.

```html
<form action="/submit" method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required>

  <label for="password">Password:</label>
  <input type="password" id="password" name="password" required>

  <label>
    <input type="checkbox" name="terms" required> I agree to terms
  </label>

  <button type="submit">Register</button>
</form>
```

---

## Part 3: Tables

**Task:** Create a table listing 3 of your favorite books.

**Requirements:**

* Use `<table>`, `<thead>`, `<tbody>`, `<tr>`, `<th>`, `<td>`.
* Include columns for Title, Author, Year.

```html
<table>
  <thead>
    <tr>
      <th>Title</th>
      <th>Author</th>
      <th>Year</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Book 1</td>
      <td>Author 1</td>
      <td>2020</td>
    </tr>
    <tr>
      <td>Book 2</td>
      <td>Author 2</td>
      <td>2018</td>
    </tr>
  </tbody>
</table>
```

---

## Part 4: Multimedia

**Task:** Embed an audio and video file.

**Requirements:**

1. Add a video using `<video>` with controls.
2. Add an audio file using `<audio>` with controls.
3. Provide a fallback message.

```html
<video width="320" controls>
  <source src="movie.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>
```

---

## Part 5: Accessibility

**Task:** Make your webpage more accessible.

**Requirements:**

1. Add meaningful `alt` attributes to all images.
2. Add ARIA labels to buttons or navigation where necessary.
3. Ensure form elements have proper `<label>` associations.

```html
<img src="logo.png" alt="Company Logo">
<button aria-label="Close Menu">X</button>
```

---

## Submission

* Combine all tasks into **one HTML file**.
* Name the file `classwork_week2_3.html`.
* Ensure proper indentation and semantic structure.
* Test for accessibility using a screen reader or browser dev tools.

**End of Classwork**
