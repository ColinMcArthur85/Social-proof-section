# Frontend Mentor - Social proof section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the section depending on their device's screen size

### Screenshot

![](./docs/images/Social%20Proof%20Screenshot.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- SASS
- CUBE CSS Methodology

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

Building out using CUBE CSS is a GAMECHANGER! I feel that aside from a few minor hiccups I was able to build this project without any issues. CUBE CSS forces you to use the cascade to your advantage so I was able to set most of the settings globally with only a few utility classes required to add finishing touches. This is such a helpful tool and I finally feel like I have a strategy rather than throwing spaghetti at a wall and hoping it will stick.

I also used SASS partials to my advatage to organize the project and then tie it all together when ready. HELPFUL!!

Below is an example of the structure of building out the layout (composition), followed by block elements and finally a utility class for final touches.

```html
<h1>Some HTML code I'm proud of</h1>
```

```scss
.//mixins
@mixin flex($direction) {
  display: flex;
  flex-direction: $direction;
}

//composition
.container {
  padding: $size-800;
  max-width: $max-width;

//utility
.flow > * + * {
   margin-top: var(--flow-space, 1em);
  }

//block
.reviews,
.intro {
   margin-bottom: $size-900;
  }
```

Was also able to seen in a data-type selector in the global settings

```css
img {
  &[data-type="star-icon"] {
    width: $size-600;
  }
  &[data-type="profile-headshot"] {
    border-radius: 50%;
    margin-right: $size-500;
    width: $size-900;
  }
}
```

Also got to use the built in color module with SASS

```scss
background: lighten($clr-primary-400, 73.5);
```

### Continued development

Continuing on with more SASS

## Author

- Frontend Mentor - [@ColinMcArthur85](https://www.frontendmentor.io/profile/ColinMcArthur85)
