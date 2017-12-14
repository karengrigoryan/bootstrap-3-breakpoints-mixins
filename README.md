# Bootstrap 3 breakpoints @mixins
Useful `scss` @mixins for easy integration of Bootstrap 3 breakpoints

> With Bootstrap 4 we got new super-useful @mixins for @media breakpoints such as `media-breakpoint-up`, `media-breakpoint-down`, etc.
> So, I've created similar @mixins that can be used in your projects based on Bootstrap 3.

## Usage
Include `mixin-breakpoints.scss` in your project and then use the following @mixins.

#### media-breakpoint-up(breakpoint)
###### SCSS
```scss
body {
  @include media-breakpoint-up(md) {
    background-color: red;
  }
}
```

###### Compiled CSS
```css
@media (min-width: 992px) {
  body {
    background-color: red;
  }
}
```

#### media-breakpoint-down(breakpoint)
###### SCSS
```scss
body {
  @include media-breakpoint-down(lg) {
    background-color: green;
  }
}
```

###### Compiled CSS:
```css
@media (max-width: 1199px) {
  body {
    background-color: green;
  }
}
```
