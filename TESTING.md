# TESTING.md - You Are Seen

This file documents all testing conducted on  **You Are Seen** project to ensure functionality, responsiveness, accessibility, and compatibility. It includes validation results, user story testing, bugs encountered, and their resolutions.

---

## Table of Contents
- [Overview](#overview)
- [Testing Strategy](#testing-strategy)
- [User Stories Testing](#user-stories-testing)
- [Functionality Testing](#functionality-testing)
- [Responsiveness Testing](#responsiveness-testing)
- [Browser Compatibility Testing](#browser-compatibility-testing)
- [Performance and Lighthouse Scan](#performance-and-lighthouse-scan)
- [Validator Results](#validator-results)
- [Bugs and Fixes](#bugs-and-fixes)
- [Additional Notes](#additional-notes)

---

##  Overview

The goal of testing was to ensure that the site behaves as expected across different devices and browsers, is accessible, and adheres to semantic and modern coding standards.

---

## Testing Strategy
- Manual testing on multiple screen sizes and devices
- Use of online validators (W3C HTML & CSS)
- Testing modal functionality and keyboard accessibility
- Confirmation of feedback display and element visibility

---

## User Stories Testing

### 1. As a user who is overwhelmed, I want to write freely without judgment.
- A clearly labeled check-in form is provided.
- Input is not stored, just acknowledged by a modal popup.

### 2. As a visitor exploring mental health resources, I want to feel welcomed and supported.
-  Resources page displays national and local support services.
- Images and messaging are calm, neutral, and inclusive.

### 3. As a returning user, I want easy navigation and reassurance.
- Navbar is simple and accessible on all screen sizes.
- Footer contains reassurance messaging and icons.

### 4. As a user, I want to view the site clearly on any device I’m using.
- Site is responsive and adapts to mobile, tablet, and desktop views.
---

##  Functionality Testing

| Feature                       | Test Case                                         | Result |
|-----------------------------|--------------------------------------------------|--------|
| Navbar links                | Clickable and navigate correctly                 |  Tested and Fully functional |
| Emotional Check-In form     | Displays modal upon submission                   | Tested and Fully functional |
| Modal (Bootstrap)           | Opens with keyboard and closes with ESC/Click   | Tested and Fully functional |
| Footer social icons         | Link to respective external pages                | Tested and Fully functional   |
| Resources links             | Open in a new tab (target="_blank")             | Tested and Fully functional |

---
### Functionality Testing Updates
- Modal activates correctly after form submission.
- Modal closes on user click of "Close" or outside the modal.
- Submission clears textarea after confirming.
- JavaScript input validation prevents special characters like `@`, `#`, `%`, `<`, etc. from being submitted.

---

##  Responsiveness Testing

Tested on the following devices:
- iPhone 
- Samsung Tab
- Windows Chrome, Edge
- Android Chrome

### Results:
- All content adapted well on each screen size
- Modal and navigation bar worked properly at all breakpoints
- Images scaled correctly without overflow

---
## Responsiveness Testing Updates
Tested on devices of varying sizes:

-  **iPhone  (Safari & Chrome)** – All sections scale correctly; modal behaves as expected.
- **Samsung (Chrome)** – Images and navbar remain responsive.
- **Windows (Chrome, Edge)** – Layout and modal display correctly.
- **iPad (Safari)** – Navigation expands cleanly; content and images stack as expected.
- **Desktop screens (1000px+ and 1200px+)** – Hero image padding scales; cards no longer appear cropped.

Screenshots included in README show layout across dark theme, mobile, tablet, and desktop views.

---
### Navigation Testing Updates:
- All internal links redirect to the appropriate section or page.
- Navigation remains sticky and consistent across pages.
- Navbar logo is now replaced with dynamic site title ("You Are Seen" or "Resources") for better readability and accessibility.
- Navigation logo/title always links back to the homepage.

---

##  Browser Compatibility Testing

| Browser      | Result |
|-------------|--------|
| Chrome       | Tested and working on Chrome   |
| Safari       | Tested and working on Safari   |
| Microsoft Edge | Tested and working on Microsoft Edge |

---

## Performance and Lighthouse Scan
A Lighthouse report was conducted, and the following issues were identified and addressed:

###  Meta Description Missing
- **Fix:** Added `<meta name="description">` to improve SEO and content summarization.

###  h1 in section lacks font-size
- **Fix:** font-size added in CSS for all heading levels to prevent browser future changes.

### Heading Order Not Sequential
- **Fix:** Headings were checked and resolved (e.g., no jumping from `<h1>` to `<h3>`).

###  DOM Size Optimization
- **Fix:** Removed redundant wrappers and unnecessary nested.


###  Oversized Images
  - **Fix:**
 Images resized using [Ezgif.com](http://ezgif.com/) and [TinyPNG](https://tinypng.com/)
Compressed to appropriate dimensions 

---
## Validator Results

### HTML
- Tested with [W3C HTML Validator](https://validator.w3.org/)
- Minor issues found and resolved:
- Stray `</div>` tag
- Unclosed `<h1>`

### CSS
- Tested with [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
-  No errors found

Screenshots included in README shows validation results.

---

## Bugs and Fixes

| Bug | Description | Fix Applied |
|-----|-------------|-------------|
| Navbar logo overflow | Logo spilled outside header in some viewports | Removed shadow and resized image |
| Modal not visible | Previous confirmation used `d-none` | Replaced with Bootstrap modal |
| Heading warnings | Inconsistent h1–h3 structure | Corrected to follow semantic order |
| Images slow to load | Images were 3–5MB each | Compressed and resized to ~300–700KB |
| Box shadow layout issue | Navbar pushed elements unexpectedly | Adjusted CSS stacking context and cleaned up rules |
| Image cropping | Cards appeared cropped on large screens | Added media queries for `min-width: 1000px+` and adjusted height |
| Hero image text not visible | Text over dark image lacked contrast | Added `.custom-text { color: white; }` styling |
| Form misuse | Users could enter special characters in journal | JavaScript validation added to restrict symbols like `@` |
| Incomplete screen support | Media query did not include screens over 1000px | Added custom queries for large devices |

---

## Summary
The project has been tested extensively across screen sizes, devices, and browsers. All performance warnings were either resolved or documented with fallback solutions. User stories were cross-checked to ensure all needs were fulfilled by the site functionality and flow.

The final product is a calm, inclusive, and technically sound platform for emotional reflection — accessible, responsive, and user-centered.

---

## Additional Notes

- Wireframes were created by the developer using **Canva Whiteboard** and tested during layout planning.
- Accessibility was considered from the start: keyboard navigation, semantic HTML, and proper ARIA usage were applied.
- Testing was conducted throughout development, not only at the end.

---

 **Created by Forest Eloghosa**
GitHub: https://github.com/Forest-Eloghosa
