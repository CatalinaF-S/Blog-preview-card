# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

-   [Overview](#overview)
    -   [The challenge](#the-challenge)
    -   [Screenshot](#screenshot)
    -   [Links](#links)
-   [My process](#my-process)
    -   [Built with](#built-with)
    -   [What I learned](#what-i-learned)

## Overview

### The challenge

Build a blog preview card according to a style guide in figma and following the "mobile first" principle using SASS as a compiler of CSS code.

### Screenshot

![Screenshot](/assets/images/screenshot.jpg)

### Links

-   Solution URL: [GitHub repository](https://github.com/CatalinaF-S/Blog-preview-card).
-   Live Site URL: [Live version](https://catalinaf-s.github.io/Blog-preview-card/).

## My process

### Built with

-   Semantic HTML5 markup
-   CSS custom properties
-   Mobile-first workflow
-   SASS (variables, mixins, styles components)

### What I learned

This challenge refreshed my knowledge of SASS and mobile first design. To use SASS, I had to remember how to install it in my project, update the scripts in package.json to run the SASS compiler, and organize the file hierarchy properly.

It was also really interesting to modularize the files I used for variables, mixins, and styles.

Here are some steps to configure my project (I write them down just to reinforce my knowledge 😊):

1. Create a project file:
   Yes, it is obvious, but sometimes you just start working in any place.

1. Installing Node.js and npm

Initialize project IN project file (i.e. in the terminal, navigate to your project file with `cd'):

```bash
npm init -y
```

This will create a package.json in my project. Then I need to install SASS (or some other package - side note to my future self 😊).

2. Installing SASS:

```bash
npm install sass --save-dev
```

3. Configure a script to run SASS:

```json
"scripts": {
  "sass": "sass --watch scss:css"
}
```

The command `--watch` runs SASS in observation mode. This means that each time you save the `.scss` file, SASS will automatically compile it into a `.css` file.

4. Create CSS and SCSS folders:

It's important to keep an eye on the folder structure of the project. All SASS-related documents will go in the `scss` folder, and when it's time to compile, the CSS documents will go in the `css` folder. Don't forget to create a CSS folder!

```bash
mkdir scss
mkdir css
touch scss/styles.scss
```

The structure should be something like this:

```
my-project/
├── scss/
│   ├── styles.scss
│   └── _variables.scss
├── css/
│   └── styles.css
├── package.json
└── node_modules/
```

5. Compilate:

To compilate just use:

```bash
npm run sass
```

And now you can beginn to code into your `.scss` file and modularizate your project as suitable for you.

Note: Don't forget to link your `.css` into your `.html`:

```html
<link rel="stylesheet" href="css/styles.css" />
```
