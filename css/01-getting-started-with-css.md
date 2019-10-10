# Getting started with CSS

## Syntax

CSS rules are created using a selector (in this case `p`) and a list of properties (in this case `font-size: 12px`.)

```css
p {
  font-size: 12px;
}
```

## Selectors

### The element selector

```html
<html>
  <head>
    <style>
      p {
        color: red;
      }
    </style>
  </head>
  <body>
    <p>Charles John Huffam Dickens was an English writer and social critic.</p>
  </body>
</html>
```

### The id selector

```html
<html>
  <head>
    <style>
      #biography {
        color: red;
      }
    </style>
  </head>
  <body>
    <p id="biography">
      Charles John Huffam Dickens was an English writer and social critic.
    </p>
  </body>
</html>
```

### The class selector

```html
<html>
  <head>
    <style>
      .biography {
        color: red;
      }
    </style>
  </head>
  <body>
    <p class="biography">
      Charles John Huffam Dickens was an English writer and social critic.
    </p>
  </body>
</html>
```

## Combining selectors

```html
<html>
  <head>
    <style>
      .large {
        font-size: 24px;
      }

      .center {
        text-align: center;
      }
    </style>
  </head>
  <body>
    <p class="large center">
      Charles John Huffam Dickens was an English writer and social critic.
    </p>
  </body>
</html>
```

## Grouping selectors

Instead of writing:

```css
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```

you can simply write:

```css
h1,
h2,
p {
  text-align: center;
  color: red;
}
```

## Comments in CSS

```css
p {
  color: red;
  /* This is a comment */
  text-align: center;
}
```

## Ways to insert CSS

### Internal stylesheet

```html
<html>
  <head>
    <style>
      body {
        background-color: lavender;
      }

      .biography {
        color: maroon;
      }
    </style>
  </head>
  <body>
    <p class="biography">
      Charles John Huffam Dickens was an English writer and social critic.
    </p>
  </body>
</html>
```

### External stylesheet

`index.html`

```html
<html>
  <head>
    <link rel="stylesheet" type="text/css" href="styles.css" />
  </head>

  <body>
    <p class="biography">
      Charles John Huffam Dickens was an English writer and social critic.
    </p>
  </body>
</html>
```

`styles.css`

```css
body {
  background-color: lavender;
}

.biography {
  color: maroon;
}
```

### Inline styles

```html
<html>
  <body style="background-color: lavender;">
    <p style="color: maroon;">
      Charles John Huffam Dickens was an English writer and social critic.
    </p>
  </body>
</html>
```

## Colors

```css
/* The following are all equivalent: */
color: red;
color: rgb(255, 0, 0);
color: #ff0000;
color: hsl(0, 100%, 50%);
```

## Typography

```
font-family: Arial, Helvetica, sans-serif;
font-weight: bold;
font-style: italic;
font-size: 24px;
text-transformation: uppercase;
text-alignment: center;
text-decoration: underline;
line-height: 2;
letter-spacing: 1px;
color: pink;
```

## Backgrounds

```
background-color: #fff;
background-image: url('https://images.unsplash.com/photo-1501236570302-906143a7c9f8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2048&q=80');
background-repeat: no-repeat;
background-position: top center;
background-size: cover;
```

## Box model

### Display

```css
display: inline|inline-block|block;
```

### Box sizing

```css
box-sizing: content-box|border-box;
```

### Width

```css
width: 300px;
width: 100%;
width: 80vw;
```

### Height

```css
height: 300px;
height: 100%;
height: 80vh;
```

### Margin

```css
margin-top: 10px;
margin-right: 5px;
margin-bottom: 10px;
margin-left: 5px;

/* Can be also written as */
margin: 10px 5px;
```

### Padding

```css
padding-top: 10px;
padding-right: 5px;
padding-bottom: 10px;
padding-left: 5px;

/* Can be also written as */
padding: 10px 5px;
```

### Border

```css
border-style: solid;
border-width: 2px;
border-color: red;

/* Can be also written as */
border: 2px solid red;
```

### Outline

```css
outline-style: solid;
outline-width: 2px;
outline-color: red;

/* Can be also written as */
outline: 2px solid red;
```

### Overflow

```css
overflow: auto|scroll|hidden|visible;
```

### Box sizing

```css
box-sizing: content-box|border-box;
```

### Box shadow

```css
box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
```

# Learn more

- [Learn more about CSS](https://www.w3schools.com/css/default.asp)
- [Learn more about colors](https://www.w3schools.com/colors/default.asp).
- [Full list of CSS properties](https://www.w3schools.com/cssref/default.asp)

# Homework

Implement the following design with HTML and CSS: [https://scene.zeplin.io/project/5d9104d9b6c1b6025612e5b5](https://scene.zeplin.io/project/5d9104d9b6c1b6025612e5b5).

Attention to detail is very important. Use Zeplin to get all the CSS values you need.
