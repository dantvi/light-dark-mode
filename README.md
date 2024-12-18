# Light Dark Mode

This project demonstrates a light and dark mode toggle for a webpage. It is part of the course "JavaScript Web Projects: 20 Projects to Build Your Portfolio" by Zero To Mastery. The application dynamically switches between light and dark themes while preserving the user's preference using local storage.

## Table of contents

- [Light Dark Mode](#light-dark-mode)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Useful resources](#useful-resources)
  - [Author](#author)
  - [Acknowledgments](#acknowledgments)

## Overview

This project provides the following functionality:
- Toggle between light and dark mode themes.
- See changes to navigation, buttons, images, and text based on the selected mode.
- Have their theme preference saved to local storage, so it persists across sessions.

### Screenshot

![](./screenshot.png)

### Links

- Live Site URL: [DT Code](https://light-dark-mode.dtcode.se/)

## My process

### Built with

- HTML5 for structure
- CSS3 for styling
  - Flexbox and custom properties
  - Dynamic theme styling using CSS variables
- JavaScript (ES6+) for interactivity
  - DOM manipulation
  - Local storage for state persistence

### What I learned

In this project, I learned:
- How to use CSS variables to define dynamic styles for themes and switch them programmatically.
- The implementation of localStorage to save and retrieve user preferences for a seamless user experience.
- How to dynamically replace icons and image sources based on the selected theme.

Example code for switching between light and dark modes:

```js
function toggleDarkLightMode(isDark) {
    nav.style.backgroundColor = isDark ? 'rgb(0 0 0 / 50%)' : 'rgb(255 255 255 / 50%)';
    textBox.style.backgroundColor = isDark ? 'rgb(255 255 255 / 50%)' : 'rgb(0 0 0 / 50%)';
    toggleIcon.children[0].textContent = isDark ? 'Dark Mode' : 'Light Mode';
    isDark
        ? toggleIcon.children[1].classList.replace('fa-sun', 'fa-moon')
        : toggleIcon.children[1].classList.replace('fa-moon', 'fa-sun');
}
```

### Useful resources

- [CSS Variables Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) - Helped in implementing dynamic theme styles with CSS variables.
- [Web Storage API Documentation](https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API) - Provided insights on using localStorage for saving user preferences.

## Author

- GitHub - [@dantvi](https://github.com/dantvi)
- LinkedIn - [@danieltving](https://www.linkedin.com/in/danieltving/)

## Acknowledgments

Special thanks to Zero To Mastery for providing the course and project structure.
