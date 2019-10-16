# Responsive web design with media Queries

To learn more about media queries, read the following articles:

- [W3Schools - Media queries](https://www.w3schools.com/css/css3_mediaqueries_ex.asp)
- [Media queries demystified](https://www.emailonacid.com/blog/article/email-development/emailology_media_queries_demystified_min-width_and_max-width/)

### Setting the viewport

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

### Media queries

```css
@media only screen and (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

### Code together

Implement a layout that looks like this on [desktop](https://scene.zeplin.io/project/5d9104d9b6c1b6025612e5b5/screen/5da779872be3e318adc170fa), on [tablet](https://scene.zeplin.io/project/5d9104d9b6c1b6025612e5b5/screen/5da77987f72860f05e2286eb) and on [phone](https://scene.zeplin.io/project/5d9104d9b6c1b6025612e5b5/screen/5da77987430fff071a086c61).

# Transforms

To learn more about the transform property, follow this link:

- [W3Schools - Transforms](https://www.w3schools.com/cssref/css3_pr_transform.asp)

We will cover the following values:

- `translate(x,y)`
- `scale(x,y)`
- `rotate(x,y)`

# Transitions and animations

To learn more about transitions and animations, follow these links:

- [W3Schools - Transitions](https://www.w3schools.com/css/css3_transitions.asp)
- [W3Schools - Animations](https://www.w3schools.com/css/css3_animations.asp)

### Transitions

We will cover the following poperties:

- `transition`
- `transition-delay`
- `transition-duration`
- `transition-property`
- `transition-timing-function`

### Animations

We will cover the following properties:

`@keyframes`
`animation-name`
`animation-duration`
`animation-delay`
`animation-iteration-count`
`animation-direction`
`animation-timing-function`
`animation-fill-mode`
`animation`

```css
div {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example;
  animation-duration: 4s;
}

@keyframes example {
  from {
    background-color: red;
  }
  to {
    background-color: yellow;
  }
}
```

# Homework

### Basic challenge

Create a `div` with the size `width:300px and height: 200px` having `background-color: #ff1493`.
On hover it will change it's size to `width: 400px and height: 260px` and it's `background-color: #00ced1`, using a transition that is done in 1 second.

### Medium challenge

Implement the following heartbeat animation in CSS: https://dribbble.com/shots/3159519-Heart-animation.
For the hearth, just use an image from the internet like [this](https://www.pinclipart.com/picdir/middle/30-306730_file-wikifont-unie033-heart-red-svg-wikimedia-commons.png).

The animation should repeat continuously.

### Hard challenge

Implement an analogue clock using only CSS. It does not need to show the time correctly, but the hour/minute/second indicators need to move realistically.

You can see an example here: https://codepen.io/dope/full/KJYMZz, however you can implement a more basic one.
