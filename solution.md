# Solution - TKTK 

# Solution Code - Styling Practice with Mockup

<details>
<summary>Step 1 Solution – Get Familiar with the Layout</summary>
    
HTML – `index.html`

```html
<!-- STEP 1: Get Familiar with the Layout -->
<!-- index.html -->
<!-- Explore the mockup/preview; no edits required yet. -->
```

</details>

<details>
<summary>Step 2 Solution – Add Your Semantic Container Tags</summary>

HTML – `index.html`

```html
<!-- STEP 2: Add Semantic Container Tags -->
<!-- index.html -->

<!-- Replace plain text with semantic containers -->
<header>Header</header>

<main>
  <!-- Wrap each content block in a semantic container.
       Keep the existing placeholder text inside for now. -->
  <section>
    <!-- Article 1 block (text/image placeholder) stays here -->
  </section>

  <section>
    <!-- Article 2 block (text placeholder) stays here -->
  </section>
</main>

<footer>Footer</footer>
```

</details>  
<details>
<summary>Step 3 Solution – Add Your Content Tags</summary>

HTML – `index.html`

```html
<!-- STEP 3: Add Content Tags (headings, paragraphs, image) -->
<!-- index.html -->

<!-- Add a page title for the main content area -->
<main>
  <h2>Main</h2>

  <section>
    <!-- Article 1 -->
    <h3>Article 1</h3>

    <!-- Add required image with src and alt -->
    <img src="https://placehold.co/200x200" alt="Placeholder landscape">

    <!-- Wrap body copy in a paragraph -->
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua.
    </p>
  </section>

  <section>
    <!-- Article 2 -->
    <h3>Article 2</h3>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua.
    </p>
  </section>
</main>

<!-- Footer text should sit inside a paragraph -->
<footer>
  <p>Footer</p>
</footer>
```

</details>   
<details>

<summary> Step 4 Solution – Connect Your Tags to the Styles</summary>

HTML – `index.html`

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Semantic Layout</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>

    <!-- Semantic header with page title -->
    <header>
      <h1>Author Bio Page</h1>
    </header>

    <!-- Main content area -->
    <main>
      <h2>Main</h2>

      <!-- First article/section with image -->
      <section class="content-block">
        <h3>Article 1</h3>
        <img src="https://placehold.co/200x200?text=My+Photo" alt="Placeholder landscape">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
      </section>

      <!-- Second article/section with text only -->
      <section class="content-block">
        <h3>Article 2</h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
      </section>
    </main>

    <!-- Semantic footer -->
    <footer id="site-footer">
      <p>Footer</p>
    </footer>

  </body>
</html>
```

CSS – `styles.css`

```css
/* === Base Page Styling === */
body {
  font-family: sans-serif;
  margin: 2rem; /* Adds space around the entire page */
  background-color: #d2ddea; /* Soft blue background for contrast */
}

/* === Layout Containers: Header, Main, Footer === */
header,
main,
footer {
  border-radius: 8px; /* Rounded corners for all major sections */
  padding: 1.5rem 0.5em; /* Inside spacing: top/bottom and sides */
  margin-bottom: 1.5rem; /* Space between sections */
}

/* === Header Section === */
header {
  background-color: #3b5998; /* Dark blue background */
  color: white;
  text-align: center;
}

header h1 {
  font-size: 2.125rem; /* Large title text */
  font-weight: 400;     /* Normal (not bold) weight */
}

/* === Main Section === */
main {
  background-color: #fffdf7; /* Subtle off-white (personalized tweak) */
}

main h2 {
  font-size: 2rem;
  text-align: center;
}

/* === Article or Section Blocks === */
.content-block {
  margin-bottom: 2em; /* Slightly increased from default */
}

/* Image inside article */
.content-block img {
  float: left;             /* Moves image to the left of the text */
  margin-right: 1em;       /* Space between image and paragraph */
  width: 100%;             /* Responsive width (max capped below) */
  max-width: 200px;        /* Prevents image from being too wide */
  height: auto;            /* Keeps natural proportions */
  max-height: 200px;       /* Prevents image from getting too tall */
  object-fit: cover;       /* Crops image to fill box without distortion */
  border-radius: 4px;      /* Slight rounding on image corners */
}

/* Clear float after image so following text isn't squished */
.content-block::after {
  content: "";
  display: block;
  clear: both;
}

/* === Footer Section === */
#site-footer {
  background-color: #333;
  color: white;
  text-align: center;
}

#site-footer p {
  font-size: 2.125rem;
  font-weight: 400;
  margin: 0;
}
```
</details>   




<details>
<summary>Final Solution</summary>

HTML – `index.html`

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Semantic Layout</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>

    <!-- Semantic header with page title -->
    <header>
      <h1>Author Bio Page</h1>
    </header>

    <!-- Main content area -->
    <main>
      <h2>Main</h2>

      <!-- First article/section with image -->
      <section class="content-block">
        <h3>Article 1</h3>
        <img src="https://placehold.co/200x200?text=My+Photo" alt="Placeholder landscape">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
      </section>

      <!-- Second article/section with text only -->
      <section class="content-block">
        <h3>Article 2</h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
      </section>
    </main>

    <!-- Semantic footer -->
    <footer id="site-footer">
      <p>Footer</p>
    </footer>

  </body>
</html>
```

CSS – `styles.css`

```css
/* === Base Page Styling === */
body {
  font-family: sans-serif;
  margin: 2rem; /* Adds space around the entire page */
  background-color: #d2ddea; /* Soft blue background for contrast */
}

/* === Layout Containers: Header, Main, Footer === */
header,
main,
footer {
  border-radius: 8px; /* Rounded corners for all major sections */
  padding: 1.5rem 0.5em; /* Inside spacing: top/bottom and sides */
  margin-bottom: 1.5rem; /* Space between sections */
}

/* === Header Section === */
header {
  background-color: #3b5998; /* Dark blue background */
  color: white;
  text-align: center;
}

header h1 {
  font-size: 2.125rem; /* Large title text */
  font-weight: 400;     /* Normal (not bold) weight */
}

/* === Main Section === */
main {
  background-color: #fffdf7; /* Subtle off-white (personalized tweak) */
}

main h2 {
  font-size: 2rem;
  text-align: center;
}

/* === Article or Section Blocks === */
.content-block {
  margin-bottom: 2em; /* Slightly increased from default */
}

/* Image inside article */
.content-block img {
  float: left;             /* Moves image to the left of the text */
  margin-right: 1em;       /* Space between image and paragraph */
  width: 100%;             /* Responsive width (max capped below) */
  max-width: 200px;        /* Prevents image from being too wide */
  height: auto;            /* Keeps natural proportions */
  max-height: 200px;       /* Prevents image from getting too tall */
  object-fit: cover;       /* Crops image to fill box without distortion */
  border-radius: 4px;      /* Slight rounding on image corners */
}

/* Clear float after image so following text isn't squished */
.content-block::after {
  content: "";
  display: block;
  clear: both;
}

/* === Footer Section === */
#site-footer {
  background-color: #333;
  color: white;
  text-align: center;
}

#site-footer p {
  font-size: 2.125rem;
  font-weight: 400;
  margin: 0;
}
```
</details>