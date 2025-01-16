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

4. We can conditionally define CSS for different breakpoints using the CSS ``` @media ``` rule.


### css at-rules

- The at-rule is a statement that provides CSS with instructions to perform or how to behave
```css
 @[KEYWORD] (RULE); 
```
- There are many rules like 
``` @import - to import a file inside a CSS file, 
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