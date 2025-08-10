# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- See hover and focus states for all interactive elements on the page
- View the optimal layout for the interface depending on their device's screen size
- See all social media links with proper styling and interactions

### Screenshot

![Social Links Profile Card](./preview.jpg)

The screenshot shows the completed social links profile card with Jessica Randall's information, featuring a clean dark theme design with green accents and interactive social media buttons.

### Links

- Solution URL: [Profile Card](https://github.com/mzamaann-dev/CodeMentor/tree/master/profile-card)
- Live Site URL: [Live URL](https://mzamaann-dev.github.io/CodeMentor/profile-card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (CSS variables)
- Flexbox for layout
- Mobile-first responsive design
- Google Fonts (Inter font family)
- CSS transitions and hover effects
- Accessibility-focused design

### What I learned

This project reinforced several important concepts in modern web development:

**CSS Custom Properties**: I used CSS variables to maintain consistent colors and typography throughout the project, making it easy to update the design system:

```css
:root {
  --green: hsl(75, 94%, 57%);
  --white: hsl(0, 0%, 100%);
  --grey-700: hsl(0, 0%, 20%);
  --grey-800: hsl(0, 0%, 12%);
  --grey-900: hsl(0, 0%, 8%);
}
```

**Responsive Design**: Implemented a mobile-first approach with proper breakpoints to ensure the design looks great on all screen sizes:

```css
@media (min-width: 768px) {
  .profile-card {
    max-width: 384px;
    padding: 40px;
  }
}
```

**Accessibility**: Added proper focus states and reduced motion support for better accessibility:

```css
.social-link:focus {
  outline: 2px solid var(--green);
  outline-offset: 2px;
}

@media (prefers-reduced-motion: reduce) {
  .social-link {
    transition: none;
  }
}
```

**Interactive Elements**: Created smooth hover effects with transforms and box shadows for a modern user experience:

```css
.social-link:hover,
.social-link:focus {
  background-color: var(--green);
  color: var(--grey-900);
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(117, 255, 0, 0.3);
}
```

### Continued development

Moving forward, I plan to focus on:

- **Advanced CSS Grid layouts** for more complex page structures
- **CSS animations and micro-interactions** to enhance user experience
- **Performance optimization** techniques for faster loading times
- **Advanced accessibility features** like ARIA labels and keyboard navigation
- **CSS preprocessors** like Sass for more maintainable stylesheets

### Useful resources

- [CSS Custom Properties Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) - Comprehensive guide on CSS variables and their best practices
- [Inter Font Family](https://fonts.google.com/specimen/Inter) - The official Google Fonts page for Inter, which helped me understand the font weights and implementation
- [CSS Flexbox Complete Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Excellent resource for mastering Flexbox layouts
- [Web Accessibility Guidelines](https://www.w3.org/WAI/WCAG21/quickref/) - Essential resource for creating accessible web content
- [CSS Media Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries) - Detailed documentation on responsive design breakpoints

## Author

- Frontend Mentor - [@mzamaann-dev](https://www.frontendmentor.io/profile/mzamaann-dev)
- GitHub - [@mzamaaann-dev](https://github.com/mzamaaann-dev)
- LinkedIn - [Muhammad Zaman](https://linkedin.com/in/yourprofile)

---

This project was completed as part of the Frontend Mentor challenges to improve HTML and CSS skills. The design follows the provided style guide and includes all required interactive states and responsive behavior.
