# USE TAILWINDCSS (3.0.23)
## SOURCE
  - https://tailwindcss.com/docs/installation

## PREREQUISITES
  - Application initialized with NPM/Yarn/etc.
  - `npm init` && `git init`
  - `npm i -D tailwindcss@3.0.23`

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

## Step Four
  - begin the Tailwind CLI build process
    - `npx tailwindcss -i ./input.css -o .dist/output.css --watch`
      - Do this instead in scripts for package.json:
        - `"watch": "tailwindcss -i ./input.css -o ./css/main.css --watch",`
        - `"build": "tailwindcss -i ./input.css -o ./css/main.css",`