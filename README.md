# USE TAILWINDCSS (3.0.23)
## PREREQUISITES
  - Application initialized with NPM/Yarn/etc.
  - `npm init` && `git init`
  - `npm i -D tailwindcss[@3.0.23]`

## Step One
  - `npx tailwindcss init`
  - creates a tailwind.config.js file

## Step Two
  - add in our content to target for the project
    - `content: ['./*.*']` or `content: ['./*.html']`.

## Step Three
  - create an `input.css` file, main project stylesheet
    - include the tailwindcss libraries as CSS imports
      - `@tailwind base;`
      - `@tailwind components;`
      - `@tailwind utilities;`