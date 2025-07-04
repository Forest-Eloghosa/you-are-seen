# You Are Seen


## Live Site

[Visit You Are Seen](https://forest-eloghosa.github.io/you-are-seen/)

A Safe Inclusive Space for Emotional Reflection and Growth

---

## Table of Contents

- [Project Description](#description)
- [User Stories](#user-stories)
- [Design and Features](#design-and-features)
- [Technologies Used and Accessibility](#technologies-used-and-accessibility)
- [Optimisations and Refactors](#optimisations-and-refactors)
- [Deployment](#deployment)
- [Testing](#testing)
- [Functionality](#functionality)
- [Responsiveness](#responsiveness)
- [Browser Compatibility](#browser-compatibility)
- [Validators](#validators)
- [Bug Fixes & Improvements](#bug-fixes--improvements)
- [Credits, Resources and Acknowledgements](#credits-resources-and-acknowledgements)
- [Feedback](#feedback)


---
## Description

“You Are Seen” is a front-end wellness and reflection site created to provide a peaceful, non-judgmental space where users can express their thoughts and emotions freely. Inspired by my lived experience and the day-to-day struggles of life, this site offers a soft landing spot for anyone and everyone to simply be.

Whether you're looking to vent, reflect, or just breathe, You Are Seen is a place where there is no pressure to be okay—and no advice unless you ask for it.

---

## User Stories

 User Needs

- As a user who is overwhelmed, I want to write freely without judgment.
- As a visitor exploring mental health resources, I want to feel welcomed and supported.
- As a returning user, I want easy navigation and reassurance that the platform is safe.
- As a user, I want to view the site clearly on any device I’m using.
---

## Design and Features
### Wireframes

Initial wireframes were created for mobile-first responsiveness. Final implementation includes adaptive layout and padding for:

- Mobile
- Tablet
- Desktop

### Fonts

- **Headings**: `DM Serif Display`
- **Body Text**: `Poppins`

### Colour Palette

| Color             | Purpose                              |
| ----------------- | ------------------------------------ |
| #a4c2d1           | Background (Egg Blue - calming tone) |
| #1f7798           | Buttons and Highlights (Mid Blue)    |
| #fce4ec           | Modal Background (Soft Pink)         |
| #ffffff / #f8f9fa | Navbar & Footer                      |

### Responsiveness

Screenshots below show responsiveness:

- iPhone & Samsung
- Desktop
- Dark Theme

---
## Wireframes

Wireframes were created using **Canva Whiteboard**.

### Tablet/Mobile:
![Tablet and Mobile](assets/images/tablet-mobile-wireframe.png "Wireframes")





### Desktop:
![Desktop](assets/images/desktop-wireframe.png "Wireframes")


---

## Features

- Emotional Check-In text box with Bootstrap modal feedback
- Mental Health Resources page with national support contacts
- Responsive layout for mobile, tablet, and desktop
- Semantic HTML for accessibility
- Soft-pink styled modal with rounded corners for gentle UX
- Footer with contact icons and copyright

---

## Technologies Used and Accessibility

### Technologies Used

- **HTML5** – Structured and semantic content
- **CSS3** – Custom styling with soft visuals
- **Bootstrap 5** – Grid layout, modal component
- **Font Awesome** – Icons for guidance
- **Canva** – Wireframe and image generation
- **JavaScript** – Form validation and modal functionality


---

### Accessibility

- Descriptive `alt` text on all images
- Semantic elements like `<header>`, `<main>`, `<section>`, `<footer>`
- ARIA attributes such as `aria-labelledby` for modals
- High contrast text and background colours
- Keyboard navigation support
- Minimal animations

---

## Optimisations and Refactors

- Made footer sticky with Flexbox layout
- Used Bootstrap utility classes: `d-flex`, `ms-auto`, `p-0`, `m-0`
- Centered hero and resource images
- Replaced original hidden confirmation div with Bootstrap modal
- Resolved layout/stacking issue due to `box-shadow`
- Removed site title from navbar and placed above hero image
- Validated and fixed HTML errors (stray `</div>`, unclosed `<h1>`, spacing)
- Validated CSS – No errors found

### Final Performance Optimisations (Post-Lighthouse Scan)

- **Meta Description Added:** Improved SEO and content discoverability.
- **Heading Font Size Fix:** Applied consistent font-size for `<h1>` in `<section>` to avoid browser rendering issues.
- **DOM Optimization:** Removed redundant `<div>` wrappers to reduce DOM complexity and improve load speed.
- **Image Resizing:** Replaced large image files with optimized versions (~300–700KB), resized for responsiveness and performance.
- **Responsive Images:** Added media queries and `object-fit` to ensure images display correctly on all devices.
- **Validated HTML and CSS:** All pages passed W3C validation with no remaining issues.

---

## Deployment

### Live Site

[Live Project on GitHub Pages](https://forest-eloghosa.github.io/you-are-seen)

### GitHub Deployment Steps

1. Fork the repository or clone using:

```bash
git clone https://github.com/Forest-Eloghosa/you-are-seen.git
```

2. Navigate into the folder:

```bash
cd you-are-seen
```

3. Make changes and push them:

```bash
git add .
git commit -m "Your message"
git push origin main
```

4. Enable GitHub Pages in repo Settings → Pages → Source → main → /root

---

## Testing
For full testing documentation, see [TESTING.md](TESTING.md)

### Functionality

- All links and buttons were tested to ensure functionality
- Bootstrap modal confirms emotional check-in submission
- Modal opens and clears form input correctly
- Special characters blocked from submission

### Responsiveness

- Site tested on multiple devices in both light and Dark theme:
- iPhone 
- Samsung Tab 
- Windows Chrome, Edge
- Android Chrome

![Responsiveness Testing](assets/images/tested-on-dark-screen-theme.jpg "tested-on-dark-screen-theme")

---

![Standard and Wide](assets/images/tested-on-large-screen.png "tested-on-large-screen")

### Browser Compatibility

- Tested and working on Chrome
- Tested and working on Firefox
- Tested and working on Safari
- Tested and working on Microsoft Edge

![Browser Compatibility Testing](assets/images/tested-on-multiple-sites-updated-image.png "tested-on-multiple-sites")

### Validators

- HTML5: [W3C Validator](https://validator.w3.org/) – all pages passed after adjustments

![HTML5 Validation](assets/images/home-page-check-in-validation.png "HTML5 Validation")

![HTML5 Validation](assets/images/home-page-check-in-validation.png "HTML5 Validation")

- CSS: [Jigsaw CSS Validator](https://jigsaw.w3.org/css-validator/) – no errors found

![CSS Validation](assets/images/css-validation.png "CSS Validation")

### Lighthouse Scan
![Lighthouse Performance](assets/images/Lighthouse-scan.png "Lighthouse Performance")
---

## Bug Fixes & Improvements
### Bug Fixes 

- **Navbar logo issue**: Fixed by removing conflicting `box-shadow`.
- **Confirmation message visibility**: Replaced with Bootstrap modal.
- **Stray **``** and open \*\*\*\***``: Fixed on both pages after validator feedback.
- **Unused CSS rules**: Removed to improve performance.
- **Missing Responsive Images**  :Images loaded full size even on smaller devices-Media queries and object-fit added.
- **Hero Padding and Background** Padding inconsistent across large screens-Media queries added to control spacing and center background.
- **Small Screen Table Spacing** Table hugged screen edge on very small devices-Media query added at max 425px for horizontal padding.
- **Bootstrap Override on Text** `.text-muted` was overriding hero text color Removed class to allow custom white styling.

These updates improved the site's performance, accessibility, and usability across all devices and browsers.

---
## Credits, Resources and Acknowledgements

### Credits
---
### Content:

- Written by Forest Eloghosa, inspired by lived experiences with emotional wellness and advocacy.

### Images:
- All images used are either license-free from [Pexels](https://pexels.com) or - [Cosmos](https://www.cosmos.so)

### Icons:
- Icons sourced from [Font Awesome](https://fontawesome.com/).

### Tools:
- Images resized using [Ezgif.com](http://ezgif.com/) and [TinyPNG](https://tinypng.com/)
Compressed to appropriate dimensions 
- [Readme Editor Tool](https://readme.so/editor "Readme Editor Tool") - For easy README creation
- [Favicon Generator](https://favicon.io/ "Favicon Generator") – For generating favicons
- [Canva for Wireframes and Logo](https://www.canva.com "Canva") – For creating wireframes and logos
- [Google Fonts](https://fonts.google.com/) – For custom fonts

### Resources

- Helplines from [ineedhelp.ie](https://ineedhelp.ie/helplines.php "Helplines")

- Helpful resources from [W3Schools HTML Forms](https://www.w3schools.com/html/html_forms.asp "W3Schools HTML Forms")

- Layout tips referenced from [MDN Web Docs](https://developer.mozilla.org/)

---
### Acknowledgements

- Special thanks to [Bootstrap](https://getbootstrap.com/) for their extensive documentation and components.
- Gratitude to [MDN Web Docs](https://developer.mozilla.org/) for their invaluable resources on web development.
- Thanks to [Code Institute](https://codeinstitute.net/) for their guidance and support throughout the project.
---
## Feedback

If you have any feedback, feel free to reach out:

- [LinkedIn](https://www.linkedin.com/in/forest-eloghosa-b16ab81ba)
- [GitHub](https://github.com/Forest-Eloghosa)