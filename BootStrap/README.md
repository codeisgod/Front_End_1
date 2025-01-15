# Introduction to Responsive Web Design*
<ol>
<li>A responsive website "responds" according to the screen size it is being rendered on.</li>
<li>Designers generally provide mockups of a website which tell a developer how the website should look on different screens.</li>
<li>To style the elements on the page depending on the screen size, we use the @media query in CSS.</li>
</ol>

## Ground Rules of responsive design

Use relative units (like rem, %) in place of absolute units (px, pt)
Use fluid containers for content as much as you can (i.e. flexbox)
Try not to use fixed width and heights, use min- or max- counterparts instead.
Design Mobile First - Mobiles are generally single column → Less CSS to be written.
Start with a small screen, then test on larger devices and see where the design "breaks", then add a breakpoint
Use @media queries to define breakpoints of a page.