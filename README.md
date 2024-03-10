
# ![Logo](https://static-00.iconduck.com/assets.00/tailwind-css-icon-512x64-vzqzx6f0.png)

#### Tailwind CSS is a powerful utility-first CSS framework that allows you to rapidly build modern websites directly in your HTML. Unlike traditional frameworks like Bootstrap, Tailwind doesn’t provide predefined classes for specific elements (such as buttons or tables). Instead, it offers a comprehensive set of utility classes that you can mix and match to style your design elements.


## Tailwindcss Link

### Site Link

```http
  https://tailwindcss.com/
  ```
### installation Link
```http  
  https://tailwindcss.com/docs/installation
```

# Install Tailwind CSS in HTML 

### First initialize the npm cmd
The command npm init -y is a convenient way to initialize an npm package without going through an interactive setup process.

```http
 npm init -y
```
### Install Tailwind CSS:
 Install tailwindcss via npm, and create your __tailwind.config.js file__.

```http
npm install -D tailwindcss
npx tailwindcss init
```
### Configure your template paths:

Add the paths to all of your template files in your __tailwind.config.js file__.
```http
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
__./src/**/*.{html,js}__ src means where the html and css file is stored.when the html and css file are stored in folder name like public change the path in src to public
```http
content: ["./public/**/*.{html,js}"],
```
if you don't create a folder use this
```http
content: ["./**/*.{html,js}"],
```
### Add the Tailwind directives to your CSS:
#### Create create a new css file and paste this cmd
#### Add the __@tailwind__ directives for each of Tailwind’s layers to your main CSS file.
```http
@tailwind base;
@tailwind components;
@tailwind utilities;
```
### Start the Tailwind CLI build process:
Run the CLI tool to scan your template files for classes and build your CSS.
```http
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```
or use this
```http
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```
or either use in __package.json__file also
```http
  "scripts": {
    "build": "npx tailwindcss -i ./style.css -o ./output.css --watch"
  },
```
## Tailwindcss Link

### Site Link

```http
  https://tailwindcss.com/
  ```
### installation Link
```http  
  https://tailwindcss.com/docs/installation
```

# Install Tailwind CSS in HTML 

### First initialize the npm cmd
The command npm init -y is a convenient way to initialize an npm package without going through an interactive setup process.

```http
 npm init -y
```
### Install Tailwind CSS:
 Install tailwindcss via npm, and create your __tailwind.config.js file__.

```http
npm install -D tailwindcss
npx tailwindcss init
```
### Configure your template paths:

Add the paths to all of your template files in your __tailwind.config.js file__.
```http
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
__./src/**/*.{html,js}__ src means where the html and css file is stored.when the html and css file are stored in folder name like public change the path in src to public
```http
content: ["./public/**/*.{html,js}"],
```
if you don't create a folder use this
```http
content: ["./**/*.{html,js}"],
```
### Add the Tailwind directives to your CSS:
Add the __@tailwind__ directives for each of Tailwind’s layers to your main CSS file.
```http
@tailwind base;
@tailwind components;
@tailwind utilities;
```
### Start the Tailwind CLI build process:
Run the CLI tool to scan your template files for classes and build your CSS.
```http
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```
or use this
```http
npx tailwindcss -i ./src/input.css -o ./public/output.css --watch
```
or either use in __package.json__file also
```http
  "scripts": {
    "build": "npx tailwindcss -i ./style.css -o ./output.css --watch"
  },
```
### Running test

Run through this command

```http
npm run build
```
or directly add command in terminal

```http
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```
