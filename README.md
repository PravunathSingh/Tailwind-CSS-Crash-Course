## Tailwind CSS Crash Course.

Tailwind is a utility-first CSS framework. In contrast to other CSS frameworks like Bootstrap or Materialize CSS it doesn’t come with predefined components. Instead Tailwind CSS operates on a lower level and provides you with a set of CSS helper classes. By using this classes you can rapidly create custom design with ease. Tailwind CSS is not opinionated and let’s you create you own unique design.

### This repo consits of a Demo Project built using the most important utility classes of Tailwind CSS. These classes can be combined with other classes available in the framework to create custom components. To read the complete documentation visit [here](https://tailwindcss.com/docs/installation).

To get started with Tailwind CSS: 

- Step 1
```
mkdir projectName
cd projectName
code .
```
- Step 2
In the project directory run the following command;

```
npm init -y
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
```
The above commands initalizes the package.json files and installs Tailwind CSS in your project.

- Step 3
Create a src and a public folder and then create a styles.css file in the src folder. This file is used to generate all the predifned styles in a styles.css file which will be generated in the public folder.

- Step 4
Add the following rules in your styles.css file. 

```
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
```
- Step 5
In the package.json file, under the scripts add the following: "build-css": "tailwindcss build src/styles.css -o public/styles.css".
And then run the following command

```
npm run build-css
```
This generates all the required CSS. And now we are ready to use all the utility classes.

#### NOTE: Every time we add our custom CSS or add custom classes we need to re-run the "npm run build-css" command.

