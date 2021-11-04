# Easybank Landing Page

This landing page has been made as a challenge from [Frontend Mentor](https://www.frontendmentor.io/challenges/easybank-landing-page-WaUhkoDN).

![](./preview.jpg)

## What I've learned

* [Responsive Design](https://www.w3schools.com/html/html_responsive.asp)
* [Sass](https://sass-lang.com/)

### Responsive Design

```scss
.container {
  @include breakpoint-up(large) {
    display: flex;
    align-items: center;
  }
}
```

### Sass variables, mixins, partials, etc.

```scss
// Partial files import
@import "hero";

// Variables
$darkBlue: hsl(233, 26%, 24%);

// Map
$breakpoints-up: ("medium": "40em", "large": "64em","xlarge": "87.5em");

// Mixins
@mixin breakpoint-down($size) {
    @media(max-width: map-get($breakpoints-down, $size)) {
        @content;
    }
}
```