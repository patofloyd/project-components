
*- Inline menu that switches to toggle menu on smaller devices*

*- Designed as a Spacecraft Starterkit compatible component*

[Here is a styleguide for this component and the rest in it's theme](https://spc-component-library.herokuapp.com/)

## About
Add the amount of menu-items that´s in your custom menu to spc\_inline_menu.config.json and it will divided and lined up inline forming a fullwidth menu. Add submenu items under your menu items and they´ll dropdown on hover, yet there is no support for items wrapped under sub-menu items. On smaller devices the menu will toggle from the menu button and expand the whole menu scrollable.

## Install

### Spacecraft Starterkit
If you have not yet installed [Spacecraft Starterkit](https://github.com/pedric/spacecraft-starterkit) , do so by running:

`git clone git@github.com:pedric/spacecraft-starterkit.git`

`cd spacecraft-starterkit`

`npm install`

### spc_article
If you have already installed [Spacecraft Starterkit](https://github.com/pedric/spacecraft-starterkit), run:

`npm install --save spc_inline_menu && gulp import --component spc_inline_menu`

And don't forget to import the css by adding:

`@import "views/spc_inline_menu/spc_inline_menu";`

in

`./src/scss/components/_components.main.scss`

## Root
Export the path with `module.exports = __dirname;` in your index.js file so that the [import tasks](https://github.com/pedric/spacecraft-starterkit#import-components) in Spacecraft can reach your files.

Care about your friends by setting up changelog-, license- and readme files for your component.

## Folders

### Docs
Add a markdown for your component that will be visible in the documentation for the styleuide. [Here is an example](https://spc-component-library.herokuapp.com/docs/spc_testfile.html).

### Icons
SVG icons goes here. Components that not uses any icons can skip this folder.

### Img
Images goes here. Probably there will be some placeholder images here, provide guidelines and info in the [documentation](#docs). Components that not uses any images can skip this folder.

### js
Here you'll put Javascript for the component, in Spacecraft you can (and are suggested to) isolate your JS to the component by making a module as [described here](https://github.com/pedric/spacecraft-starterkit#javascript).

### View
This is the place for:

• HTML (Twig)

• CSS (SCSS)

• Config (JSON)

Twig is Spacecraft´s default but Nunjucks, Handlebars etc can be used. This is set in Spacecraft´s config for your project.