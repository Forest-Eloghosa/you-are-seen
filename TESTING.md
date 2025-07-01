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

---

##  Functionality Testing

| Feature                       | Test Case                                         | Result |
|-----------------------------|--------------------------------------------------|--------|
| Navbar links                | Clickable and navigate correctly                 |  100% |
| Emotional Check-In form     | Displays modal upon submission                   | 100%     |
| Modal (Bootstrap)           | Opens with keyboard and closes with ESC/Click   | 100%    |
| Footer social icons         | Link to respective external pages                | 100%     |
| Resources links             | Open in a new tab (target="_blank")             | 100%     |

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

##  Browser Compatibility Testing

| Browser      | Result |
|-------------|--------|
| Chrome       | 100%   |
 Safari       | 100%   |
| Microsoft Edge | 100% |

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

---

##  Bugs and Fixes

### 1. **Navbar Logo Positioned Incorrectly**
- **Issue**: Logo appeared outside nav bar on some screen sizes
- **Fix**: Removed conflicting `box-shadow` styling in custom CSS

### 2. **Confirmation Message Not Visible**
- **Issue**: Original hidden `div` went unnoticed after submitting form
- **Fix**: Replaced with a Bootstrap modal that visually confirms submission

### 3. **Aria-labelledby Not Connected Properly**
- **Issue**: Modal’s `aria-labelledby` attribute was not pointing to any element
- **Fix**: Connected it to the `id` of the modal title element

---

## Additional Notes

- Wireframes were created by the developer using **Canva Whiteboard** and tested during layout planning.
- Accessibility was considered from the start: keyboard navigation, semantic HTML, and proper ARIA usage were applied.
- Testing was conducted throughout development, not only at the end.

---

 **Created by Forest Eloghosa**
GitHub: https://github.com/Forest-Eloghosa
