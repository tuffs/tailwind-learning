# SETUP FOR TAILWINDCSS @ v. 3.0.23
## Step One
  - `npx tailwindcss init`
  - creates a tailwind.config.js file

## Step Two
  - add in our content to target for the project
    - `content: ['./*.*']` or `content: ['./*.html']`.

## Step Three
  - create an input.css (or whatever you'd like to call it)
    - thought is to include the tailwindcss libraries as imports
      - `@tailwind base;`
      - `@tailwind components;`
      - `@tailwind utilities;`