# Building the Network Github Template
## What is Network?

Network is a GitHub template designed by @rudrathegreat.

## Developing the HTML
### The HTML Skeleton

To start, we're just going to type up the HTML skeleton - 

```HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" type="text/css" href="style.css">
    <title>Title</title>
</head>
<body>
</body>
</html>

```
### The navbar

Next, we're going to type up the navigation bar in html. A pretty standard method to making a navigation bar is the one shown below -

```HTML

<header>
        <input type="checkbox" class="nav-toggle" id="nav-toggle">
        <div class="hamburger">
            <div class="bar"></div>
        </div>
        <h1 class="logo">R</h1>
            <nav class="nav">
            <ul class="nav-list">
                <li class="nav-list-element"><a href="" class="nav-link">Home</a></li>
                <li class="nav-list-element"><a href="" class="nav-link">About</a></li>
                <li class="nav-list-element"><a href="" class="nav-link">Blog</a></li>
                <li class="nav-list-element"><a href="" class="nav-link">Contacts</a></li>
            </ul>
        </nav>
    </header>

```

So, how is the navigation bar structured and what do each of the elements do? Well, we have a header, which is simply a container in which we are going to have our navigation bar in. Inside the header, we have a checkbox followed by a div labelled 'hamburger'. This is going to form the hamburger icon, which will allow our navigation to be responsive on mobile devices. Inside the header, we also have our nav. This is the navigation bar, and inside it, we have all the things we find in a navigation bar (logo, links, etc).

### The title

Next we'll add the title, along with the subtitle and a background image -

```HTML

<div class="title" style="background-image:url("background.jpg");">
        <h1>Title</h1>
        <h2>Subtitle</h2>
        <a class="link-to-about" onclick="document.getElementById('text-and-image').scrollIntoView(true);">
            <i class="fas fa-chevron-down"></i>
        </a>
    </div>

```

Again, let's try and understand the code. We have a container labelled 'title' which has a background image with the filename background.jpg. Inside the container, we have our title, followed by our subtitle, followed by a button. This button is a 'down arrow button' and the button comes from a site called fontawesome.com. In order for the button to work, we need to add the following line - 

```HTML

    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.4.1/css/all.css">

```

inside our head tags (add it underneath the line where we link the CSS file).

### Text only section

Let's add some text to our website - 

```HTML

<div class="text-only" id="text-only">
        <h1>Heading</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem sed risus ultricies tristique nulla aliquet. Maecenas volutpat blandit aliquam etiam erat velit scelerisque in dictum. Porta nibh venenatis cras sed felis eget velit. Imperdiet proin fermentum leo vel orci porta non. Tincidunt tortor aliquam nulla facilisi cras fermentum. Hendrerit gravida rutrum quisque non tellus orci. Nec nam aliquam sem et tortor. Bibendum arcu vitae elementum curabitur vitae nunc sed. A iaculis at erat pellentesque. Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices. Quam vulputate dignissim suspendisse in est ante. Sit amet facilisis magna etiam tempor orci eu lobortis elementum. Porttitor massa id neque aliquam vestibulum morbi.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem sed risus ultricies tristique nulla aliquet. Maecenas volutpat blandit aliquam etiam erat velit scelerisque in dictum. Porta nibh venenatis cras sed felis eget velit. Imperdiet proin fermentum leo vel orci porta non. Tincidunt tortor aliquam nulla facilisi cras fermentum. Hendrerit gravida rutrum quisque non tellus orci. Nec nam aliquam sem et tortor. Bibendum arcu vitae elementum curabitur vitae nunc sed. A iaculis at erat pellentesque. Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices. Quam vulputate dignissim suspendisse in est ante. Sit amet facilisis magna etiam tempor orci eu lobortis elementum. Porttitor massa id neque aliquam vestibulum morbi.</p>
        <a>Learn More</a>
    </div>

```

Again, let's try and understand the code. We have a container by the name of 'text-only'. Inside it, we have 2 paragraphs followed by a button that says 'learn more'.

### Text and image section

Let's add some more text, but this time with an image - 

```HTML

<div class="text-and-image" id="text-and-image">
        <h1>Heading</h1>
        <table class="desktop">
            <tr>
                <td>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem sed risus ultricies tristique nulla aliquet. Maecenas volutpat blandit aliquam etiam erat velit scelerisque in dictum. Porta nibh venenatis cras sed felis eget velit. Imperdiet proin fermentum leo vel orci porta non. Tincidunt tortor aliquam nulla facilisi cras fermentum. Hendrerit gravida rutrum quisque non tellus orci. Nec nam aliquam sem et tortor. Bibendum arcu vitae elementum curabitur vitae nunc sed. A iaculis at erat pellentesque. Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices. Quam vulputate dignissim suspendisse in est ante. Sit amet facilisis magna etiam tempor orci eu lobortis elementum. Porttitor massa id neque aliquam vestibulum morbi.</p>
                    <a>Learn More</a>
                </td>
                <td><img src="{{background}}"></td>
            </tr>
        </table>
        <table class="mobile">
            <tr><td>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem sed risus ultricies tristique nulla aliquet. Maecenas volutpat blandit aliquam etiam erat velit scelerisque in dictum. Porta nibh venenatis cras sed felis eget velit. Imperdiet proin fermentum leo vel orci porta non. Tincidunt tortor aliquam nulla facilisi cras fermentum. Hendrerit gravida rutrum quisque non tellus orci. Nec nam aliquam sem et tortor. Bibendum arcu vitae elementum curabitur vitae nunc sed. A iaculis at erat pellentesque. Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices. Quam vulputate dignissim suspendisse in est ante. Sit amet facilisis magna etiam tempor orci eu lobortis elementum. Porttitor massa id neque aliquam vestibulum morbi.</p>
                <a>Learn More</a>
            </td></tr>
            <tr><td><img src="{{background}}"></td></tr>
        </table>
    </div>

```

Let's try and understand this one. We first have a container called 'text-and-image'. Inside it, we have our heading followed by 2 tables.

The first table (labelled 'desktop') has 1 row. Inside the 1 row, there are two cells. One of the cells contain a paragraph followed by a button that says 'learn more'. In the other table cell, we have an image. When the website is open on a laptop, then users will see this table.

The second table (labelled 'mobile') has two rows. Inside each row, there is only one cell. Inside the first row, there's our text, and in the second row is our image. When the website is viewed on a phone, then the users will see this table.

### A Footer

Let's finally add a footer - 

```HTML

<div class="footer">
        <p>Copyright &copy; 2020. Organisation name. All Rights Reserved.</p>
    </div>

```

We have a container labelled 'footer' and inside it we have our copyright statement.

## Developing the CSS
### Basic CSS properties

We'll first add the following CSS lines to make sure that there is no unnecessary spacing - 

```CSS

* {
    margin:0;
    padding:0;
}

```

Followed by a line to style the scroll-behaviour in the website - 

```CSS

html {
    scroll-behavior:smooth;
}

```

### Scrollbar Properties

Nobody wants a default scrollbar, so let's add some CSS to make our own custom scrollbar -

```CSS

::-webkit-scrollbar {
    width:10px;
    background:#eee;
}

::-webkit-scrollbar-thumb {
    background:#ef4d8c;
    border-radius:10px;
}

```

Let's break this down. A scrollbar consists of 2 elements, the bar and the scroll-y thing that allows you to scroll a page when you click and drag it up and down. We're first setting the width of the scrollbar to 10px, then setting the background of the **bar** to a very light-grey. Then, we're setting the colour of the scroll-y thing to a shade of pink and adding a bit of curvature to the corners to the scroll-y thing.

### Body

Let's just set up a basic font which is going to be used throughout the website along with a default background - 

```CSS

body {
    font-family:'Raleway', sans-serif;
    background:#000;
}

```

### The Navbar

Just for a recap, here's the HTML structure of the navigation bar - 

```HTML

<header>
        <input type="checkbox" class="nav-toggle" id="nav-toggle">
        <div class="hamburger">
            <div class="bar"></div>
        </div>
        <h1 class="logo">R</h1>
            <nav class="nav">
            <ul class="nav-list">
                <li class="nav-list-element"><a href="" class="nav-link">Home</a></li>
                <li class="nav-list-element"><a href="" class="nav-link">About</a></li>
                <li class="nav-list-element"><a href="" class="nav-link">Blog</a></li>
                <li class="nav-list-element"><a href="" class="nav-link">Contacts</a></li>
            </ul>
        </nav>
    </header>

```

We're going to take things one step at a time, styling one element after another.

#### The Header

The first step is to style the header, inside of which is our navigation bar - 

```CSS

header {
    width:100%;
    height:100px;
    background:#fff;
    text-transform:uppercase;
    text-decoration:none;
    list-style:none;
    position:fixed;
    top:0;
    left:0;
    z-index:10;
    box-shadow: 0vh 0vh 25px #000000;
    text-align:center;
}

```

Firstly, we're setting up the dimensions of the header so that it stretches the full width of the screen and has a height of 100px. We're setting the background to white. We're making sure that text inside of our header is capitalised and that there is no text decoration on that text (no underlines, etc.). Next, we're fixing the position of the header (and everything inside it), making sure it is at the top of our screen. We're making sure that the navbar is on top of everything else using the z-index property. Then, we're adding a shadow to the header followed a text-align:center;

#### The Logo

Now, let's style the logo - 

```CSS

.logo {
    color:#333;
    position:absolute;
    top:50%;
    transform:translateY(-50%);
    margin-left:2em;
    font-weight:800;
    transition: color 0.1s ease-in-out, transform 0.1s ease-in-out;
}

.logo:hover {
    transform:scale(1.1) translateY(-50%);
    color:#ef4d8c;
    transition: color 0.1s ease-in-out, transform 0.1s ease-in-out;
}


```

Ok, so firstly we're setting the font colour to a dark grey. Next, we're setting the position to absolute. Setting the position to absolute allows us to freely position the logo. In the next two lines, we're vertically centering the logo. Then , we're adding some space to the left of the logo in the line `margin-left:2em;`. Next, we're setting the font-weight (the bigger the font-weight, the more bold a text is).In the lines below, we're adding a :hover statement. That means, when users hover over the logo using their mouse, some CSS will change. That css in the font colour and the size of the logo (the logo is scaled by a factor of 1.1).

#### The Hamburger

Now, let's add the CSS for the hamburger icon - 

```CSS

.nav-toggle {
    position:absolute;
    top:0;
    z-index:15;
    right:0;
    margin-right:3em;
    align-items:center;
    height:100%;
    width:5vw;
    opacity:0;
    display:none;
}

.hamburger {
  height: 100%;
  position: absolute;
  top: 0;
  right: 0;
  z-index: 14;
  display: none;
  margin-right:3em;
  justify-content: center;
  align-items: center;
  box-sizing: border-box;
  transition: all 0.3s ease-in-out;
}

.bar::before,
.bar::after,
.bar {
    width: 5vw;
    height:3px;
    background:#000;
}

.bar {
    position:relative;
    display:block;
}

.bar::before,
.bar::after {
    content:'';
    position:absolute;
    left:0;
    transition:all 0.3s ease-in-out;
}

.bar::after {
   transition:all 0.3s ease-in-out;
}

.bar::before {
    top:10px;
}

.bar::after {
    bottom:10px;
}

.nav-toggle:checked + .hamburger {
        transform: rotate(45deg);
        transform-origin:middle;
        transition:all 0.3s ease-in-out;
}

.nav-toggle:checked + .hamburger .bar::before,
.nav-toggle:checked + .hamburger .bar::after {
  top: 0;
  transform-origin:middle;
  transform: rotate(90deg);
  transition: transform 0.3s ease-in-out;
}

.nav-toggle:checked + .hamburger .bar::after {
    opacity:0;
    transition:opacity 0.3s ease-in-out;
}

.nav-toggle:checked ~ nav {
    display:block;
    font-size:4vw;
    transform:scale(1,1);
    transition: transform 0.5s ease-in-out;
}

.nav-toggle:checked ~ nav a {
    color:#000;
    opacity:1;
    transition:color 0.3s ease-in-out, opacity 0.5s ease-in-out 0.3s;
}

.nav-toggle:checked ~ nav a:hover {
    color: #ef4d8c;
    transition:color 0.2s ease-in-out;
}

```

Most of the CSS above is simply there to create a hamburger icon, to position the checkboxes and hamburger, etc, to animate the hamburger when clicked upon. The most important piece of CSS are the following sections - 

```CSS

.nav-toggle:checked ~ nav {
    display:block;
    font-size:4vw;
    transform:scale(1,1);
    transition: transform 0.5s ease-in-out;
}

.nav-toggle:checked ~ nav a {
    color:#000;
    opacity:1;
    transition:color 0.3s ease-in-out, opacity 0.5s ease-in-out 0.3s;
}

.nav-toggle:checked ~ nav a:hover {
    color: #ef4d8c;
    transition:color 0.2s ease-in-out;
}

```

The CSS above contains the following statements - 

- If the hamburger is checked, then apply the following CSS to the nav. In this scenario, when the hamburger icon is checked, then the nav will open up.
- If the hamburger is checked, then apply the following CSS to the links inside the nav. In this case, when the hamburger icon is checked, then show all the links and change the font settings.
- If the hamburger is checked and the user's mouse is hovering over one of the links, then apply the following CSS to that link. In this scenario, when the hamburger icon is checked and the user's mouse is hovering over one of the links, then the font colour of that link will change.

#### Styling Nav, Nav-list and Nav-link

The nav container is simply going to take the shape of its parent container 'header' - 

```CSS

.nav {
    width:100%;
    height:100%;
}

```

Next, let's add the CSS for the nav-list (the list containing all the links which is inside the nav) - 

```CSS

.nav-list {
    display:flex;
    height:100%;
    gap:3em;
    margin-left:13em;
    text-decoration:none;
    list-style:none;
    align-items:center;
    color:#000;
}

```

We're first using the property of `display:flex;` to evenly space out all the elements inside the nav-list. Next, we're giving it a height of 100%. After that, we're spacing out each of the links inside the list by 3em. We're giving the list a margin of 13em to the left. We're making sure there is no text-decoration and that there are no dot points (`list-style:none;` removes all dot points from lists). Then we're vertically aligning the links in the center of the navigation bar and setting the font colour of the links to black.

Next, let's style the nav-links - 

```CSS

.nav-link {
    color:#000;
    text-decoration:none;
    font-weight:700;
    transition:color 0.2s ease-in-out;
}

.nav-link:hover {
    color:#ef4d8c;
    transition:color 0.2s ease-in-out;
}

```

We're first setting the color of the nav-links to black and the text-decoration to none. We're making the nav-links bolder by increasing the font weight. When the user hovers on the nav-link, then the color changes to that shade of pink, with a nice, smooth transition.

And that's the navigation bar!

### The title

Remember that this is the HTML structure of our title - 

```HTML

<div class="title" style="background-image:url("background.jpg");">
        <h1>Title</h1>
        <h2>Subtitle</h2>
        <a class="link-to-about" onclick="document.getElementById('text-and-image').scrollIntoView(true);">
            <i class="fas fa-chevron-down"></i>
        </a>
    </div>

```

Let's style the container encompassing the title, subtitle and down arrow button - 

```CSS

.title {
    width:100%;
    height:100vh;
    display:flex;
    margin:0;
    flex-direction:column;
    background-size:cover;
    background-position:center;
    background-attachment:fixed;
    background-repeat:no-repeat;
    color:#fff;
    align-items:center;
    justify-content:center;
    text-align:center;
    text-transform:uppercase;
    letter-spacing:3px;
}

```

The CSS might seem like a lot, but's it actually not! We're first setting up the dimensions of the container container the title, subtitle, etc. In this case, we're setting the dimensions of the container to be the same as the screen itself. Next, we're evenly spacing out all the elements inside the container, making sure there are no margins. The background image is filling the entire container and we're positioning the background image in the center of the container. Then, we're fixing it in that position, allowing for a simple parallax effect. Then, we make sure that the background image is not repeating itself in the container. We align all the items inside the container in the center (both vertically and horizontally), making sure that our text is capitalised and has a letter spacing of 3px.

Now, let's style the title, subtitle and the down arrow - 

```CSS

.title h1 {
    color:#fff;
    font-size:6vw;
    font-weight:900;
    text-transform:uppercase;
}

.title h2 {
    font-size:2.5vw;
    padding-top:1vh;
    text-transform:uppercase;
    font-weight:700;
    color:#fff;
}

.title a {
    position:absolute;
    top:80%;
    left:50%;
    transform:translate(-50%, -50%);
    transition:top 0.2s ease-in-out;
    color:#fff;
}

.title a:hover {
    top:81%;
    transition:top 0.2s ease-in-out;
}

```

Let's start with the title. We're setting the font colour to white, the font size to 6vw and the font-weight to 900 (**ULTRA BOLD** xD) and capitalising all the letters in the title. With the subtitle (h2), we're setting the font-size to 2.5vw, adding a slight space of 1vh between the title and the subtitle, capitalising the subtitle, setting the font-weight to 700 and setting the colour to white. The first 4 lines styling the down arrow button are effectively horizontally positioning the button. After that, we're setting the colour of the down arrow button to white. When the user hovers over the down arrow button, it will go down by 1% of the screen size, with a nice transition of 0.2s.

### Text-only section

Let's recall that this is the HTML structure of our text-only section - 

```HTML

<div class="text-only" id="text-only">
        <h1>Heading</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem sed risus ultricies tristique nulla aliquet. Maecenas volutpat blandit aliquam etiam erat velit scelerisque in dictum. Porta nibh venenatis cras sed felis eget velit. Imperdiet proin fermentum leo vel orci porta non. Tincidunt tortor aliquam nulla facilisi cras fermentum. Hendrerit gravida rutrum quisque non tellus orci. Nec nam aliquam sem et tortor. Bibendum arcu vitae elementum curabitur vitae nunc sed. A iaculis at erat pellentesque. Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices. Quam vulputate dignissim suspendisse in est ante. Sit amet facilisis magna etiam tempor orci eu lobortis elementum. Porttitor massa id neque aliquam vestibulum morbi.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem sed risus ultricies tristique nulla aliquet. Maecenas volutpat blandit aliquam etiam erat velit scelerisque in dictum. Porta nibh venenatis cras sed felis eget velit. Imperdiet proin fermentum leo vel orci porta non. Tincidunt tortor aliquam nulla facilisi cras fermentum. Hendrerit gravida rutrum quisque non tellus orci. Nec nam aliquam sem et tortor. Bibendum arcu vitae elementum curabitur vitae nunc sed. A iaculis at erat pellentesque. Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices. Quam vulputate dignissim suspendisse in est ante. Sit amet facilisis magna etiam tempor orci eu lobortis elementum. Porttitor massa id neque aliquam vestibulum morbi.</p>
        <a>Learn More</a>
    </div>

```

Let's add the CSS - 

```CSS

.text-only {
    text-align:center;
    width:100%;
    height:100vh;
    background:#eee;
    color:#333;
    display:flex;
    flex-direction:column;
    gap:3vh;
    justify-content:center;
    align-items:center;
}

.text-only h1 {
    font-weight:800;
    font-size:5vw;
    color:#ef4d8c;
}

.text-only p {
    font-size:1.25vw;
    line-height:1.5;
    width:80%;
    font-weight:500;
}

.text-only a {
    font-family:sans-serif;
    text-transform:uppercase;
    font-weight:700;
    padding:1vh 2vw;
    border: 3px solid #ef4d8c;
    font-size:1.5vw;
    color:#cd2b6a;
    transition:background 0.2s ease-in-out, color 0.2s ease-in;
}

.text-only a:hover {
    color:#fff;
    background:#ef4d8c;
    transition:background 0.2s ease-in-out, color 0.2s ease-in;
}

.text-only a {
    border-radius:3vw;
    padding:1.5vh 2vw;
}

```

First, we're styling the container which has the text in it. It's going to take the shape of the window and have a light grey background and a font-colour of a dark grey. We're spacing out all items inside the container vertically and then aligning them to the center of the container while giving a gap of 3vh. For our heading, we're setting a font-weight of 800, then we're setting the font-size to 5vw and a color of pink. For the paragraphs, we're setting a font-size of 1.25vw, then we're spacing out each of the lines in the paragraphs 1.5x more than it usually would, and then we're setting the font-weight to 500. With the button, we're first setting all the font settings (font-family, text-transform, etc.). We're then adding some space around the text, followed by a border of 3px. When the user hovers over the button, the background will change to a pink colour and the font colour will change to a white colour.

### Text and Image Section

Here's the text and image section in its HTML structure - 

```HTML

<div class="text-and-image" id="text-and-image">
        <h1>Heading</h1>
        <table class="desktop">
            <tr>
                <td>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem sed risus ultricies tristique nulla aliquet. Maecenas volutpat blandit aliquam etiam erat velit scelerisque in dictum. Porta nibh venenatis cras sed felis eget velit. Imperdiet proin fermentum leo vel orci porta non. Tincidunt tortor aliquam nulla facilisi cras fermentum. Hendrerit gravida rutrum quisque non tellus orci. Nec nam aliquam sem et tortor. Bibendum arcu vitae elementum curabitur vitae nunc sed. A iaculis at erat pellentesque. Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices. Quam vulputate dignissim suspendisse in est ante. Sit amet facilisis magna etiam tempor orci eu lobortis elementum. Porttitor massa id neque aliquam vestibulum morbi.</p>
                    <a>Learn More</a>
                </td>
                <td><img src="{{background}}"></td>
            </tr>
        </table>
        <table class="mobile">
            <tr><td>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem sed risus ultricies tristique nulla aliquet. Maecenas volutpat blandit aliquam etiam erat velit scelerisque in dictum. Porta nibh venenatis cras sed felis eget velit. Imperdiet proin fermentum leo vel orci porta non. Tincidunt tortor aliquam nulla facilisi cras fermentum. Hendrerit gravida rutrum quisque non tellus orci. Nec nam aliquam sem et tortor. Bibendum arcu vitae elementum curabitur vitae nunc sed. A iaculis at erat pellentesque. Pretium aenean pharetra magna ac placerat vestibulum lectus mauris ultrices. Quam vulputate dignissim suspendisse in est ante. Sit amet facilisis magna etiam tempor orci eu lobortis elementum. Porttitor massa id neque aliquam vestibulum morbi.</p>
                <a>Learn More</a>
            </td></tr>
            <tr><td><img src="image.jpg"></td></tr>
        </table>
    </div>

```

Let's style this up using some CSS - 

```CSS

.text-and-image {
    width:100%;
    height:100vh;
    background:#eee;
    color:#333;
    margin:0;
    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;
}

.text-and-image table {
    width:80%;
    padding-top:5vh;
}

.text-and-image tr {
    width:100%;
}

.text-and-image td {
    width:50%;
    display:table-cell;
    flex-direction:column;
    align-items:center;
    justify-content:center;
}

.text-and-image img {
    width:90%;
    margin-left:5%;
}

.text-and-image a {
    font-family:sans-serif;
    text-transform:uppercase;
    font-weight:700;
    padding:1vh 2vw;
    border: 3px solid #ef4d8c;
    font-size:1.5vw;
    color:#cd2b6a;
    transition:background 0.2s ease-in-out, color 0.2s ease-in;
}

.text-and-image a:hover {
    color:#fff;
    background:#ef4d8c;
    transition:background 0.2s ease-in-out, color 0.2s ease-in;
}

.text-and-image h1 {
    font-weight:800;
    font-size:5vw;
}

.text-and-image p {
    font-size:1.25vw;
    line-height:1.5;
    font-weight:500;
    padding-bottom:5vh;
}

```

Let's take this one by one. We first have our text-and-image container, which takes the shape of the window, background of light grey, a font colour of dark grey, no margins and evenly spaces out all the elements inside it, centering the elements in the center of the container. Inside the container, we have a table, which has a width of 80% of its parent container and a space between it and the heading of 5vh. We have the row, which takes up 100% of the width of the table, and then the table cell, which takes up 50% of the row. All the elements inside the table cell are being centered and evenly spaced out in the table cell. We then style the image, having a width 90% that of the table cell, and margin to the left of the image. We then style the button, exactly the same as how we did above, except without the curved edges. We're then styling the heading and the paragraphs, exactly the same as with our text-only section.

### Footer

The footer is simply a container surrounding our copyright statement. Let's style it up -

```CSS

.footer {
    width:100%;
    height:10vh;
    background:#000;
    color:#fff;
    font-size:1.25vw;
    text-transform:uppercase;
    text-align:center;
    font-weight:700;
    display:flex;
    align-items:center;
    justify-content:center;
}

.footer p {
    width:100%;
}

```

We're first styling the container, making it so that stretches the full width of the window, but only has a height 10% that of the window. The background is set to black, and the font-colour is set to white. We're changing the font settings, then aligning our copyright statement in the center of the footer. Then, with the copyright statement, we want it to stretch the full width of the footer so that it is aligned in the center of the footer.

### Mobile Responsive

Let's add the code to make the website mobile responsive - 

```CSS

.mobile {
    display:none;
}

@media screen and (max-width: 900px) {
    ::-webkit-scrollbar {
        width:0px;
        background:#eee;
    }
    header {
        height:100px;
    }

    .nav-toggle {
        display:block;
    }
    .nav {
        width:100%;
        height:100vh;
        background:#fff;
        transform:scale(1,0);
        transform-origin:bottom;
        display:block;
        transition: transform 0.5s ease-in-out 0.2s;
    }

    .nav-list {
        display:flex;
        flex-direction:column;
        justify-content:center;
        width:100%;
        font-size:4vw;
        margin-left:0;
        gap:3em;
        text-decoration:none;
        color:#000;
    }

    .nav-link {
        text-decoration:none;
        color:#000;
        opacity:0;
        transition: opacity 0.3s ease-in-out;
    }

    .hamburger {
        display:flex;
    }

    .nav-desktop {
        display:none;
    }

    .logo {
        z-index:20;
    }

    .desktop {
        display:none;
    }

    .mobile {
        display:table;
        padding-top:10vh;
    }

    .mobile p {
        font-size:2vw;
        text-align:center;
        padding-bottom:3vh;
    }

    .title {
        text-align:center;
    }

    .title h1 {
        padding-left:0;
    }

    .title h2 {
        padding-left:0;
    }

    .title img {
        width:80%;
    }

    .text-only p {
        font-size:2vw;
    }

    .footer {
        font-size:2vw;
    }

    .text-and-image tr {
        width:100%;
    }

    .text-and-image td {
        width:100%;
        display:flex;
    }

    .text-and-image a {
        font-size:2.5vw;
        margin-bottom:3vh;
    }

    .text-only a {
        font-size:2.5vw;
        border-radius:5vw;
        padding:1.5vh 3vw;
    }

    .text-and-image img {
        margin-left:0;
        width:70%;
    }
}


``` 
Most of the CSS here just changes the font sizes when on small screens, reorders elements to fit everything on tiny screens, etc. However, this is the most important line - 

```CSS

@media screen and (max-width: 900px) {
}

```

This line basically translates to 'if the window size is smaller than 900px, then apply the CSS inside this condition'. That's ho we're making the website mobile responsive. WE DID IT!

## Problems along the way
### Latest CSS not applied on HTML

Sometimes, when you add CSS, save it and then refresh the browser to see the changes, you don't see any. That's because there's not enough space in your cache to process the new CSS. To fix it, just clear your cache. On Chrome, simply go to History, then click on 'Clear Browsing History'. Select the cache option and click 'Ok'.

# Thanks for Reading!
