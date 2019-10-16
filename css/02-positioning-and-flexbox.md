# The position property

There are five different position values in CSS:

```
static
relative
fixed
absolute
sticky
```

### position: static;

HTML elements are positioned static by default.
An element with position: static; is not positioned in any special way; it is always positioned according to the normal flow of the page:

```css
.static {
  position: static;
  border: 3px solid #73ad21;
}
```

### position: relative;

An element with `position: relative;` is positioned relative to its normal position.

```html
<div class="relative">
  This element has position: relative;
</div>
```

```css
.relative {
  position: relative;
  left: 30px;
  border: 3px solid #73ad21;
}
```

### position: fixed;

An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.

```html
<div class="fixed">
  This element has position: fixed;
</div>
```

```css
div.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 100%;
  border: 3px solid #73ad21;
}
```

### position: absolute;

An element with `position: absolute;` is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like `fixed`).

However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.

```html
<div class="relative">
  This element has position: relative;

  <div class="absolute">
    This element has position: absolute;
  </div>
</div>
```

```css
.relative {
  position: relative;
  width: 400px;
  height: 200px;
  border: 3px solid #73ad21;
}

.absolute {
  position: absolute;
  top: 80px;
  right: 0;
  width: 200px;
  height: 100px;
  border: 3px solid #73ad21;
}
```

### position: sticky;

An element with `position: sticky;` is positioned based on the user's scroll position.

A sticky element toggles between `relative` and `fixed`, depending on the scroll position. It is positioned `relative` until a given offset position is met in the viewport - then it "sticks" in place (like `position:fixed`).

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      .sticky {
        position: sticky;
        top: 0;
        padding: 5px;
        background-color: #cae8ca;
        border: 2px solid #4caf50;
      }
    </style>
  </head>
  <body>
    <p>
      Try to <b>scroll</b> inside this frame to understand how sticky
      positioning works.
    </p>

    <div class="sticky">I am sticky!</div>

    <div style="padding-bottom:2000px">
      <p>
        In this example, the sticky element sticks to the top of the page (top:
        0), when you reach its scroll position.
      </p>
      <p>Scroll back up to remove the stickyness.</p>
      <p>
        Some text to enable scrolling.. Lorem ipsum dolor sit amet, illum
        definitiones no quo, maluisset concludaturque et eum, altera fabulas ut
        quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. Affert
        laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no
        molestiae voluptatibus.
      </p>
      <p>
        Some text to enable scrolling.. Lorem ipsum dolor sit amet, illum
        definitiones no quo, maluisset concludaturque et eum, altera fabulas ut
        quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. Affert
        laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no
        molestiae voluptatibus.
      </p>
    </div>
  </body>
</html>
```

# Flexbox

To better understand flexbox you can read the following articles:

- [Flexbox on W3Schools](https://www.w3schools.com/css/css3_flexbox.asp)
- [Flexbox on CSS tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [About `flex-grow` and `flex-shrink`](https://medium.com/@tiffnogueira/understanding-flex-shrink-flex-grow-and-flex-basis-and-using-these-properties-to-their-full-e4b4afd2c930)

Today, we will cover the following css properties:

### Container elements

- `flex-direction`: `row`|`row-reverse`|`column`|`column-reverse`
- `flex-wrap`: `wrap`|`no-wrap`|`wrap-reverse`
- `flex-flow` - is a shorthand property for `flex-direction` and `flex-wrap`
- `justify-content`: `flex-start`|`center`|`flex-end`|`space-between`|`space-around`
- `align-items`: `flex-start`|`center`|`flex-end`|`stretch`|`baseline`
- `align-content`: `space-between`|`space-around`|`strecth`|`center`|`flex-start`|`flex-end`

### Child elements

- `order`
- `flex-grow`
- `flex-shrink`
- `flex-basis`
- `flex` - shorthand property for `flex-grow`, `flex-shrink`, and `flex-basis`
- `align-self`

# Homework

Name your folder: `tema-03`.

## Part 1
Exercise your flexbox skills, and complete all levels of [this game](https://flexboxfroggy.com).

## Part 2
Implement the following layout using flexbox: https://scene.zeplin.io/project/5d9104d9b6c1b6025612e5b5/screen/5d9ee7cbdb5981302764c303.
