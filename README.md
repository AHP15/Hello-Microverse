# Hello-Microverse

This project is built to master all of the tools and best practices I learned about in previous steps because I will be using them in all Microverse projects and most likely in my future job as well

## Built with

* HTML/CSS
* Webhint/Stylelint

## Getting Started

This is a simple HTML page including an h1 header and a CSS file including the style for the h1

To get a local copy up and running follow these simple example steps.

## Prerequisites

* Github flow
* Basic HTML and CSS

## Setup
### Webhint

NOTE: If you are running on Windows, you need to initialize npm to create package.json file.
```bash
npm init -y
```

1. Run 
```bash
npm install --save-dev hint@7.x
```
2. create a file in the root directory of your project named .hintrc and copy the following to it
```json
  {
    "connector": {
      "name": "local",
      "options": {
        "pattern": ["**", "!.git/**", "!node_modules/**"]
      }
    },
    "extends": ["development"],
    "formatters": ["stylish"],
    "hints": [
      "button-type",
      "disown-opener",
      "html-checker",
      "meta-charset-utf-8",
      "meta-viewport",
      "no-inline-styles:error"
    ]
}
```
3. Run 
```bash
npx hint .
```
4. Fix validation errors.