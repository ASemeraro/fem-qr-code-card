# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview
I decided to tackle this challenge by using [Sass](https://sass-lang.com/) and [BEM methodology](https://en.bem.info/methodology/). I'm not too familiar with them, so I decided this challenge would be a nice way to learn.

### Screenshot

![](./images/my-solution-cover.jpg)

### Links

- Live Site URL: [Please check it out on Github Pages 🎉](https://asemeraro.github.io/fem-qr-code-card.github.io/)

## My process

### Set up sass + gulp + browsersync workflow
Although I have set up a file structure in the past with Sass, I decided to use [Yeoman](https://yeoman.io/) to generate the files necessary for the sass + gulp + browsersync workflow that I adopted in this project. The generator I used is `gulp-sass-boilerplate` by [coder-coder](https://github.com/thecodercoder/generator-gulp-sass-boilerplate).

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Sass + Gulp
- Figma (to help estimating margins and paddings for the design provided by Frontend Mentor)

### What I learned

I learned about the `hsl` colour notation and how it can be used to specify colours in a project.
`hsl` stands for __HUE__, __SATURATION__, __LIGHTNESS__.

```css
:root {
	--white: hsl(0, 0%, 100%);
	--light-gray: hsl(212, 45%, 89%);
	--grayish-blue: hsl(220, 15%, 55%);
	--dark-blue: hsl(218, 44%, 22%);
}
```

While I was trying to centre the card in the middle of the page, I discovered that the `<body>` had the same `height` as its content. I needed the `height` to span the whole page, if I wanted `flexbox` to work properly and centre the card. My solution became as follows:

```css
body {
  //...
  min-height: 100vh;
}
```

How to host on Github pages.

__Name the repo__
- Be sure to have named your repo as follows `repo-name.github.io`.
- If you need to rename it, just go to `Settings` -> `General` -> `Repository name`. Write the new name and click on `Rename`.
- At that point go back to the `<> Code` tab, click on the `Code` dropdown, copy the new link!
- In your local repo, be sure to run this command `git remote set-url origin repo-name.github.io`.

__Set repo visibility to PUBLIC__
- Be sure to set your repo to `public`.
- Go to `Settings` -> `General` -> scroll down to `Danger Zone` -> `Change repository visibility` and click on `Change visibility` -> Select `Make public` in the modal and type what is requested to confirm.

__Activate Github pages__
- Go to `Settings`.
- In the `Code and automation` section, click on `Pages`.
- Selec a branch, a folder and click on `Save`.
- That's it!!! 🎉 There will be a link to the live page soon after saving.


### Continued development

I would like to re-create this project in React. I barely started looking at React, so a project with a small scope like this one is perfect for learning purposes.

## Author

- Frontend Mentor - [@ASemeraro](https://www.frontendmentor.io/profile/ASemeraro)

## Acknowledgments

I think I wouldn't have been able to even feel confident enough to take a challenge like this, if it wasn't for [coder-coder](https://www.youtube.com/thecodercoder), a great and inspiring YouTuber. I highly recommend her channel if you are a beginner front-end developer.