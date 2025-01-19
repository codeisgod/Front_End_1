# RESPONSIVE WEB DESIGN

## Introduction to Responsive Web Design

1. A responsive website "responds" according to the screen size it is being rendered on.
2. Designers generally provide mockups of a website which tell a developer how the website should look on different screens.
3. To style the elements on the page depending on the screen size, we use the ``` @media ``` query in CSS.

## Ground Rules of Responsive Design

1. Use relative units ``` (like rem, %) ``` in place of absolute units (px, pt).
2. Use fluid containers for content as much as you can ``` (i.e., flexbox).```
3. Try not to use fixed width and heights, use ``` min- or max- ``` counterparts instead.
4. Design Mobile First - Mobiles are generally single column → Less CSS to be written.
   1. Start with a small screen, then test on larger devices and see where the design "breaks", then add a breakpoint.
   2. Use ``` @media ``` queries to define breakpoints of a page.

### Breakpoints

1. Breakpoints define the width of different screen sizes on which our website can be viewed.
2. One way to think about breakpoints is → Starting with mobile, the "point" where your design starts to "break".
3. There are some standard breakpoints used in CSS:

   - `320px` or `375px`  -> Mobile Phones
   - `480px`             -> Small tablets
   - `640px` or `768px`  -> Normal tablets
   - `960px` or `1024px` -> Laptops and Desktops
   - `1280px`            -> Hi Resolution Laptops

4. We can conditionally define CSS for different breakpoints using the CSS ` @media ` rule.


### css at-rules

- The at-rule is a statement that provides CSS with instructions to perform or how to behave
```css
 @[KEYWORD] (RULE); 
```
- There are many rules like 
``` 
@import - to import a file inside a CSS file, 
@font-face - to define local/self-hosted fonts, 
@keyframes - for animations
```

### @media Rule

To define breakpoints, we are particularly interested in the @media rule of CSS
- The @media rule allows us to define CSS for different "media"
- It is written as
    ```css
    @media [media-type] ([media-feature]) { 
    /*Styles for this media*/
    }
    ```
- When moving towards larger screens from our small screen design, we can define breakpoints as a `media-feature` for a particular `media type`

### Using @media Rule
- We will use 375px (mobile), 768px (tablet), 1024px (laptops), and 1280px (hi-res laptops)
- Define a `meta` tag in the head with `name="viewport"` like this to make your media queries work.
```css
<meta name="viewport" content="width=device-width, initial-scale=1" />
```
- Use `min-width` to define your media queries
- To define a breakpoint write a media query like ⬇️
```css
@media (min-width: 375px) {
  /*Define Styles here*/
}
```
- The above media query will allow you to define styles for screens with at least 375px of width

# BootStrap

- Bootstrap is a `CSS framework` by Twitter
It allows us to leverage `pre-written CSS classes` which we can directly use out-of-the-box
- It also gives us shorthand notations for common CSS properties like `flex, grid, margin, padding` etc.
- Bootstrap has a lot of components built in with their own CSS (and functionality using JS)

## Structure of BootStrap
- Bootstrap primarily works on the concept of CSS class selectors.
- You can attach multiple classes to any HTML element, separated by spaces.
- The structure can be mapped down to 4 main parts
   - Layout - Containers, Grid, Columns, Breakpoints, Z-Index etc
   - Content - Typography, images etc
   - Components - Pre Built components like cards, navbar, carousel, buttons etc
   - Utilities - Your plain CSS which had been writing up till now.

## How to use BootStrap

- [BootStrap](https://getbootstrap.com/)
- [BootStrap Introduction](https://getbootstrap.com/docs/5.3/getting-started/introduction/)

- Bootstrap requires two meta tags like charset and viewport which allow Bootstrap to work responsively on different screens.
```HTML
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
```

- under `head` tag use below code
```HTML
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
```
and under body tag use this Script (JS)
```HTML
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

- To view above both written code, remove `min` from link 
```
https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.css
https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.js
```

- bootstrap import two things CSS and related JavaScript

### Example Code
```HTML
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Bootstrap demo</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
  </head>
  <body>
    <h1>Hello, world!</h1>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
  </body>
</html>
```