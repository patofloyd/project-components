
*- Button with rounded corners and some hover-effects*

*- Designed as a Spacecraft Starterkit compatible component*

[Here is a styleguide for this component and the rest in it's theme](https://spc-component-library.herokuapp.com/)

## About
No config.json needed, set button-content in the `data-spc_more_button` attribute like this: `data-spc_more_button="value"` in spc_more_button.twig.

Change the color variables in scss-file to customise, by default it´s #fff and #000 set as "bright and dark". Button set to fullwidth at `@media screen and (max-width:800px)`.

## Install
Clone/download [Spacecraft Starterkit](https://github.com/pedric/spacecraft-starterkit) and run:

`npm install`

`npm install --save <component-name>`
// To get this actual component downloaded.

`gulp import --component <component-name>`
// To get the files into your project.

`gulp`
// To start up Spacecraft.

The last step is to import the css, in..

`./src/scss/components/_components.main.scss`

..add..

`@import "views/<component-name>/<component-name>";`

*- A test-/template component for Spacecraft Starterkit*

This suggests how components are to be structured and given name to be compatible with the [Spacecraft Starterkit](https://github.com/pedric/spacecraft-starterkit) and to meet good standard.

[PROJECT COMPONENTS AT GITHUB](https://github.com/pedric/project-components)

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