# Assignment 3.4 — Semantic HTML & Accessibility

**Topic:** Converting a Div-Based Webpage into Semantic HTML  
**File Name:** `index.html`

## 1. Objective

The objective of this assignment is to convert a webpage built mainly with `<div>` elements into a semantic HTML webpage. Semantic elements improve the structure, readability, accessibility, and maintainability of a website.

## 2. Before: Div-Based HTML

The following example shows a basic webpage built using `<div>` elements.

```html
<div>
    <div>
        <h1>My Portfolio</h1>
    </div>

    <div>
        <a href="index.html">Home</a>
        <a href="about.html">About</a>
    </div>

    <div>
        <h2>About Me</h2>
        <p>I am learning web development.</p>
    </div>

    <div>
        <p>Created for my assignment.</p>
    </div>
</div>
```

### Problems with the Div-Based Page

- The purpose of each section is not clearly identified by its HTML element.
- The page structure is less meaningful to assistive technologies.
- The code can be harder to understand and maintain as the page grows.

## 3. After: Semantic HTML Code

Create a file named `index.html` and paste the following code into it.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio | Semantic HTML</title>
</head>
<body>

    <header>
        <h1>My Portfolio</h1>
        <p>Welcome to my personal website.</p>
    </header>

    <nav aria-label="Main navigation">
        <a href="index.html">Home</a>
        <a href="#about">About Me</a>
        <a href="#skills">My Skills</a>
        <a href="#contact">Contact</a>
    </nav>

    <hr>

    <main>
        <section id="about">
            <h2>About Me</h2>

            <p>
                Hello! I am learning web development.
                I enjoy exploring HTML and creating
                useful and accessible webpages.
            </p>

            <figure>
                <img
                    src="https://placehold.co/300x200"
                    alt="Placeholder image representing a personal portfolio"
                    width="300"
                    height="200">
                <figcaption>My portfolio image</figcaption>
            </figure>
        </section>

        <hr>

        <section id="skills">
            <h2>My Skills</h2>

            <article>
                <h3>HTML</h3>
                <p>
                    HTML is used to structure content on webpages.
                    Semantic HTML gives meaning to different parts
                    of a webpage.
                </p>
            </article>

            <article>
                <h3>Web Accessibility</h3>
                <p>
                    Web accessibility helps people with different
                    abilities understand and use websites.
                </p>
            </article>
        </section>

        <aside>
            <h2>Learning Resource</h2>
            <p>
                Learn more about HTML from
                <a href="https://developer.mozilla.org/en-US/docs/Web/HTML"
                   target="_blank"
                   rel="noopener noreferrer">
                    MDN Web Docs: HTML
                </a>.
            </p>
        </aside>

        <hr>

        <section id="contact">
            <h2>Contact Information</h2>
            <p>
                For this assignment, you can contact me through
                the contact details provided in my portfolio.
            </p>
        </section>
    </main>

    <footer>
        <p>Created for Assignment 3.4 — Semantic HTML & Accessibility.</p>
    </footer>

</body>
</html>
```

**Note:** The image URL above is a placeholder and requires an internet connection. You can replace it with your own image, such as `images/profile.jpg`, after placing the image inside your project's `images` folder.

## 4. Semantic Elements Used

| HTML Element | Purpose |
|---|---|
| `<header>` | Contains the introductory content of the page. |
| `<nav>` | Contains navigation links. |
| `<main>` | Contains the main content of the webpage. |
| `<section>` | Groups related content under a heading. |
| `<article>` | Contains a self-contained piece of content. |
| `<aside>` | Contains related or supplementary information. |
| `<footer>` | Contains footer information. |
| `<figure>` | Groups an image or other illustrative content. |
| `<figcaption>` | Provides a caption for the image. |

## 5. Accessibility Improvements

1. Added `lang="en"` to identify the page language.
2. Used meaningful headings in a logical hierarchy: `<h1>`, `<h2>`, and `<h3>`.
3. Placed navigation links inside the `<nav>` element.
4. Placed the primary page content inside `<main>`.
5. Added meaningful alternative text using the `alt` attribute.
6. Used understandable link text instead of vague text such as “click here.”
7. Added an accessible label to the navigation using `aria-label`.

## 6. Steps to Run and Test

1. Open Visual Studio Code or Notepad.
2. Create a file named `index.html`.
3. Paste the updated semantic HTML code into the file.
4. Save the file.
5. Open it in Google Chrome or Microsoft Edge.
6. Check that the Home, About Me, My Skills, and Contact links navigate to the correct locations.
7. Click the MDN Web Docs link and verify that it opens in a new tab.
8. Check that the image appears and that the headings and page sections are understandable.

## 7. Before and After Comparison

**Before:**
- The webpage uses generic `<div>` elements for most sections.
- The purpose of each container is not explicitly described by its HTML tag.

**After:**
- The webpage uses meaningful semantic elements.
- Navigation, main content, supplementary information, and footer content are separated.
- Headings and image alternative text make the content easier to understand.

## 8. Screenshots for Submission

Take actual screenshots from your computer:

1. **Before screenshot:** Show the original div-based HTML code in your editor.
2. **After screenshot:** Show the updated semantic HTML code in your editor.
3. **Browser screenshot:** Show the finished webpage in Chrome or Edge.

Keep the original div-based example separately if you need to demonstrate the before-and-after changes.

## 9. Result

Successfully converted a div-based webpage into a semantic HTML webpage using `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, and `<footer>`. Improved the structure and accessibility by using a logical heading hierarchy, meaningful alternative text, and understandable navigation links.

## 10. Conclusion

This assignment helped me understand the importance of semantic HTML and accessibility. Semantic elements make webpages more organized, meaningful, easier to maintain, and more understandable to assistive technologies.

**Assignment 3.4 Completed Successfully.**