
````markdown
# Week 1: Setup & Web Fundamentals

## 🎯 Learning Objectives
By the end of this week, you should be able to:
- Understand the basics of how the internet works.
- Set up your coding environment (VS Code, browser, extensions).
- Write your first **HTML page** using correct structure.
- Deploy and preview your work locally.

---

## 🌍 How the Internet Works
Before we dive into coding, let’s cover the basics:

- **HTTP (HyperText Transfer Protocol):** The set of rules for transferring web pages between a browser (client) and server.
- **DNS (Domain Name System):** Translates human-friendly domain names (like `google.com`) into IP addresses.
- **Browsers:** Software (Chrome, Firefox, etc.) that interprets HTML, CSS, and JavaScript to display web pages.

📖 Recommended Read: [MDN - How the Web Works](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)

---

## 🛠️ Setup Your Development Environment

### 1. Install **VS Code**
- Download from [https://code.visualstudio.com/](https://code.visualstudio.com/).
- Install extensions:
  - **Live Server** (to preview your HTML in real-time).
  - **Prettier** (for clean formatting).

### 2. Install a Browser
- Use **Google Chrome** or **Mozilla Firefox**.
- Open **DevTools** with:
  - `Ctrl + Shift + I` (Windows/Linux)
  - `Cmd + Option + I` (Mac)

### 3. Install Git
- Download from [https://git-scm.com/downloads](https://git-scm.com/downloads).
- Verify installation:
  ```bash
  git --version
````

---

## 🏗️ Basic HTML Structure

Every HTML file follows a standard structure:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Hello World</title>
  </head>
  <body>
    <h1>Hello World 🌍</h1>
    <p>My first webpage using HTML.</p>
  </body>
</html>
```

### Explanation:

* `<!DOCTYPE html>` → Tells the browser this is an HTML5 document.
* `<html>` → Root element of the page.
* `<head>` → Contains metadata (title, charset, viewport).
* `<body>` → Where the visible content of your page goes.

---

## 📝 Assignment: Create Your First Webpage

### Task:

1. Install **VS Code**, **Git**, and your **browser**.
2. Create a new folder: `week1-hello-world`.
3. Inside it, create a file: `index.html`.
4. Add the **basic HTML structure** and write `"Hello World"` inside an `<h1>` tag.
5. Open the file with **Live Server** to preview in your browser.

### Example:

```html
<h1>Hello World from [Your Name]</h1>
<p>This is my first web page!</p>
```

---

## ✅ Marking Criteria (10 points)

| Criteria                                              | Points |
| ----------------------------------------------------- | ------ |
| Correct setup (VS Code + Live Server + Git installed) | 5 pts  |
| Working HTML page with correct structure              | 5 pts  |

---

## 📚 Extra Resources

* [MDN - HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)
* [FreeCodeCamp - Learn HTML](https://www.freecodecamp.org/learn/2022/responsive-web-design/#basic-html-and-html5)

---

## 💡 Instructor Notes

* Encourage students to **share screenshots** of their first webpage.
* Debugging tip: If Live Server isn’t working, right-click the HTML file → **Open with Live Server**.
* Prepare students for **Week 2-3: HTML Deep Dive**.

