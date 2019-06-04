# ITCSS BOILERPLATE 

This is an ITCSS boilerplate which represents a map/file structure you can use to setup new ITCSS projects.

## Features
### Numeric
Each ITCSS folder has a numeric prefix so it shown in the right order and easier to find. 

### Double underscore files
The main file in each ITCSS folder contains a double underscore so it is always shown on top. From this main file you can import other SCSS files.

## Folder structure

1. **Settings** – used with preprocessors and contain font, colors definitions, etc.

2. **Tools** – globally used mixins and functions. It’s important not to output any CSS in the first 2 layers.

3. **Generic** – reset and/or normalize styles, box-sizing definition, etc. This is the first layer which generates actual CSS.

4. **Elements** – styling for bare HTML elements (like `H1`, `A`, etc.). These come with default styling from the browser so we can redefine them here.

5. **Objects** – class-based selectors which define undecorated design patterns, for example media object known from **OOCSS**

6. **Components** – specific UI components. This is where majority of our work takes place and our UI components are often composed of Objects and Components. **BEM** is a good methology to use here. 

7. **Utilities** – utilities and helper classes with ability to override anything which goes before in the triangle, eg. hide helper class. This should be the only place were `!important` is used
 

## External resources
- https://www.xfive.co/blog/itcss-scalable-maintainable-css-architecture/ 
- [Harry Roberts - Managing CSS Projects with ITCSS](https://www.youtube.com/watch?v=1OKZOV-iLj4)
- https://en.bem.info/methodology/
