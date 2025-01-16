# RESPONSIVE WEB DESIGN

## Introduction to Responsive Web Design
<ol>
    <li>
        A responsive website "responds" according to the screen size it is being rendered on.
    </li>
    <li>
        Designers generally provide mockups of a website which tell a developer how the website should look on different screens.
    </li>
    <li>
        To style the elements on the page depending on the screen size, we use the @media query in CSS.
    </li>
</ol>

## Ground Rules of responsive design
<ol>
    <li>
        Use relative units (like rem, %) in place of absolute units (px, pt)
    </li>
    <li>
        Use fluid containers for content as much as you can (i.e. flexbox)
    </li>
    <li>
        Try not to use fixed width and heights, use min- or max- counterparts instead.
    </li>
    <li>
        Design Mobile First - Mobiles are generally single column → Less CSS to be written.
        <ol>
            <li>
                Start with a small screen, then test on larger devices and see where the design "breaks", then add a breakpoint
            </li>
            <li>
                Use @media queries to define breakpoints of a page.
            </li>
        </ol>
    </li>
</ol>

### Breakpoints
<ol>
    <li>Breakpoints define the width of different screen sizes on which our website can be viewed.</li>
    <li>One way to think about breakpoints is → Starting with mobile, the "point" where your design starts to "break"</li>
    <li>There are some standard breakpoints used in CSS.</li>
    <ul>
        <li>320px or 375px  -> Mobile Phones</li>
        <li>480px  -> Small tablets</li>
        <li>640px or 768px  -> Normal tablets</li>
        <li>960px or 1024px ->  Laptops and Desktops</li>
        <li>1280px -> Hi Resolution Laptops</li>
    </ul>
    <li>We can conditionally define CSS for different breakpoints using CSS @media rule.</li>
</ol>

### css at-rules

<ul>
    <li>
        The at-rule is a statement that provides CSS with instructions to perform or how to behave
        <br>
        @[KEYWORD] (RULE);
    </li>
    <li>
        There are many rules like @import - to import a file inside a CSS file, @font-face - to define local/self-hosted fonts, @keyframes - for animations
    </li>
</ul>

### @media Rule

To define breakpoints, we are particularly interested in the @media rule of CSS
<ul>
    <li>The @media rule allows us to define CSS for different "media"</li>
    <li>It is written as <br>
    @media [media-type] ([media-feature]) {
    /*Styles for this media*/
    }
    </li>
</ul>