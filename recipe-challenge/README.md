# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page
- View the recipe page with proper typography, colors, and spacing
- Access a responsive design that works on mobile, tablet, and desktop

### Screenshot

![Design preview for the Recipe page coding challenge](./preview.jpg)

### Links

- Solution URL: [Profile Card](https://github.com/mzamaann-dev/CodeMentor/tree/master/recipe-challenge)
- Live Site URL: [Live URL](https://mzamaann-dev.github.io/CodeMentor/recipe-challenge/)


## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (Design Tokens)
- CSS Flexbox & Grid
- Mobile-first responsive design
- CSS pseudo-elements and counters
- Google Fonts integration
- Professional CSS architecture

### What I learned

This project was an excellent opportunity to practice advanced CSS techniques and professional development practices:

**CSS Custom Properties & Design System:**
```css
:root {
  /* Colors */
  --color-white: hsl(0, 0%, 100%);
  --color-stone-100: hsl(30, 54%, 90%);
  --color-brown-800: hsl(14, 45%, 36%);
  
  /* Typography */
  --font-family-primary: 'Young Serif', serif;
  --font-family-secondary: 'Outfit', sans-serif;
  
  /* Spacing System */
  --spacing-xs: 0.5rem;
  --spacing-sm: 1rem;
  --spacing-md: 1.5rem;
}
```

**Advanced CSS Techniques:**
```css
/* Custom numbered list with CSS counters */
.instructions li::marker {
  color: var(--color-brown-800);
  font-weight: var(--font-weight-bold);
  font-size: 1rem;
}

/* Custom bullet points with pseudo-elements */
.ingredients li::before {
  content: '';
  position: absolute;
  left: 0;
  top: 1rem;
  width: 4px;
  height: 4px;
  background-color: var(--color-brown-800);
  border-radius: 50%;
}
```

**Responsive Design Patterns:**
```css
/* Mobile-first approach */
.container {
  max-width: var(--container-mobile);
}

@media (min-width: 768px) {
  .container {
    max-width: 736px;
  }
}
```

### Continued development

Areas I want to continue focusing on in future projects:

- **CSS Architecture**: Further refine my approach to organizing CSS with methodologies like BEM or ITCSS
- **Performance Optimization**: Implement CSS optimization techniques like critical CSS and code splitting
- **Accessibility**: Enhance focus management and screen reader compatibility
- **CSS Animations**: Add subtle micro-interactions and transitions for better UX
- **CSS-in-JS**: Explore modern styling solutions for larger applications

### Useful resources

- [CSS Custom Properties Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) - Comprehensive guide on CSS custom properties and their best practices
- [CSS Grid Layout](https://css-tricks.com/snippets/css/complete-guide-grid/) - Complete guide to CSS Grid for modern layouts
- [Flexbox Complete Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Essential resource for mastering Flexbox
- [CSS Pseudo-elements](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements) - Documentation on creating custom elements with CSS
- [Mobile-First Responsive Design](https://www.lukew.com/ff/entry.asp?933) - Luke Wroblewski's insights on mobile-first design

## Author

- GitHub - [@mzamaann-dev](https://github.com/mzamaann-dev)
- Frontend Mentor - [@mzamaann-dev](https://www.frontendmentor.io/profile/mzamaann-dev)
- LinkedIn - [Muhammad Zaman](https://linkedin.com/in/mzamaann)

---

**Note**: This project was built as part of the Frontend Mentor challenges to improve coding skills and build realistic projects. The design and requirements were provided by Frontend Mentor.
