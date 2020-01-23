# Getting started with HTML

## Typography

```html
<html>
  <body>
    <h1>Title of the page</h1>
    <b>Some bolded text.</b>
    <i>Some italic text.</i>
    <u>Some underlined text.</u>

    <strong>Some strong text.</strong>
    <em>Some emphasized text.</em>
    <center>Some centered text.</center>

    <blockquote>Some quoted text</blockquote>
    <del>Some deleted text</del>

    <span>Some simple text</span>

    <!-- a text break is below -->
    <br />

    <p>Some paragraph</p>
  </body>
</html>
```

## Container elements

```html
<html>
  <body>
    <div>
      <span>Hello</span>
    </div>
    <div>
      <span>World</span>
    </div>
  </body>
</html>
```

## Lists

### Ordered lists

```html
<ol>
  <li>One</li>
  <li>Two</li>
  <li>Three</li>
  <li>Four</li>
</ol>
```

### Unordered lists

```html
<ul>
  <li>One</li>
  <li>Two</li>
  <li>Three</li>
  <li>Four</li>
</ul>
```

## Description lists

```html
<dl>
  <dt>Name</dt>
  <dd>John Doe</dd>
  <dt>Age</dt>
  <dd>40</dd>
</dl>
```

## Media elements

### Figures and images

```html
<figure>
  <img src="rome.jpg" alt="Rome, Italy" />
  <figcaption>Fig.1 - Rome, Italy.</figcaption>
</figure>
```

### Audio

```html
<audio controls autoplay loop muted preload>
  <source src="file.ogg" type="audio/ogg" />
  <source src="file.mp3" type="audio/mpeg" />
  Your browser does not support the audio tag.
</audio>
```

You can use a file from here: https://s3.amazonaws.com/web-development-course-static-files/stairway-to-heaven.mp3

### Video

```html
<video width="320" height="240" controls autoplay loop muted preload>
  <source src="movie.mp4" type="video/mp4" />
  <source src="movie.ogg" type="video/ogg" />
  Your browser does not support the video tag.
</video>
```

You can use a file from here: https://s3.amazonaws.com/web-development-course-static-files/big-buck-bunny.mp4

## Elements for interaction

```html
<button disabled>Do something</button>
<a href="https://facebook.com">Link to Facebook</a>
```

## Tables

```html
<table>
  <thead>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$80</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Sum</td>
      <td>$180</td>
    </tr>
  </tfoot>
</table>
```

## Embed elements

### Iframe

```html
<iframe
  width="640"
  height="320"
  src="https://www.youtube.com/embed/aqz-KE-bpKQ"
/>
```

### Styles

```html
<html>
  <head>
    <style>
      img {
        width: 300px;
        height: 200px;
      }
    </style>
  </head>
</html>
```

#### Scripts

```html
<html>
  <head>
    <script>
      window.alert("Hi! How are you today?");
    </script>
  </head>
</html>
```

## Comments

```html
<!DOCTYPE html>
<html>
  <body>
    <!-- This is a comment -->
    <h1>Title of the page</h1>
  </body>
</html>
```

# Learn more

[List of all HTML elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

# Homework

Create a table with two columns: `month` and `balance`, and for each month of the year create a row with the name of the month (e.g. `January`) and the current balance (e.g. `$100`). Use any random values for balances.
