# NAANOVO
### Completed January 2021

**Time Frame**

I completed this project in my spare time, around my full time role. This took around 30 hours.

## Project Overview
This client wanted their site to be based very closely with the PDF of their company offerings, so the branding and content was already in place. I drafted some low fidelity wireframes for the layout so that the translation from PDF to site made sense, and users could navigate their way through easily.

This was created using mainly HTML and CSS, with a small amount of JavaScript for the mobile menu. I found myself most comfortable using CSS Flexbox and this made up a lot of the CSS styling for each page. 

You can see the full site here: [Naanovo.com](http://www.naanovo.com/)

## Technologies Used

- HTML5
- CSS3
- JavaScript

## Featured Code

### Parallax Scrolling

This was my first time using parallax scrolling and it became a feature on a lot of the site's backgrounds. 

```
header {
  width: auto;
  height: 50vh;
  background-image: url(./final-images/header-main.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  /*  Parallax Scrolling for background image  */
  background-attachment: fixed;
  background-position: bottom;
  /* ^^ */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
```

### Burger Menu

A very small amount of JavaScript was used for the mobile burger menu function, using an if/else statement and a comparison operator. 

```function myFunction() {
  var x = document.getElementById("myLinks");
  if (x.style.display === "block") {
    x.style.display = "none";
  } else {
    x.style.display = "block";
  }
}
```

### Media Queries

I needed to make sure to add edits for mobile users as some of the site's features were not compatible. The parallax scrolling and CSS hover animations were edited to be mobile friendly or replaced altogether with alternatives.

```
@media (hover: none) {
/* Fix parallax background images in place for mobile */
  header, .main-page, .tech-page, .main-team-page, .our-projects {
    background-attachment: scroll;
  }
```

## Challenges

I have a section that states the companies key values on the main page, which I wanted to make more interactive for the user. As you hover over each value title you are then shown some more copy on how the company upholds this value. I needed to have a placeholder when the page first loads and then the ability for this to be changed as you hover. This meant duplicating the first option into its own class and subsequently hiding it as the user begins to hover through the other options. In future I would look to do this animation with JavaScript.

```
<h4>Our Values</h4>
    <div class="text-hold">
      <p><span class="value-title">Family</span> is highly valued in all things that we do as a company, whether ...</p>
    </div>
    <div class="values">Family</div>
    <div class="text-container">
      <p><span class="value-title">Family</span> is highly valued in all things that we do as a company, whether ...</p>
    </div>
```

## Wins

- Parallax scrolling
- Media Queries
- Wireframing

## Key Learnings

- **Wireframing** - I found this very useful to convert the PDF I was initially given into something I could share with the client to make sure we were aligned with the look and features of the site, as well as being able to see that it was something a user could navigate through.
- **Set clear client boundaries** - I needed to have clear working hours, and a clear contact process for edits and requests. I was making this site in my free time around a full time day job, and the client would call at all hours including weekends and bank holidays no matter the size of the request.

## Future Content

- Add more JavaScript for interactivity and for flexibility, instead of being reliant on CSS options.
