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

## Step Five
  - create an `index.html` file and link the output `main.css` file.

## Step Six
  - Inside of the `tailwind.config.js` file, updates to Screens and Theme Colors
  - Example: 
    - ```
        theme: {
          screens: {
            'sm': '480px',
            'md': '768px',
            'lg': '976px',
            'xl': '1440px',
          },
          extend: {
            colors: {
              brightRed: 'hsl(12, 88%, 59%)',
              brightRedLight: 'hsl(12, 88%, 69%)',
              brightRedSupLight: 'hsl(12, 88%, 95%)',
              darkBlue: 'hsl(228, 39%, 23%)',
              darkGrayishBlue: 'hsl(227, 12%, 61%)',
              veryDarkBlue: 'hsl(233, 12%, 13%)',
              veryPaleRed: 'hsl(13, 100%, 96%)',
              veryLightGray: 'hsl(0, 0%, 98%)',
            }
          },
        }
      ```

## Setup VSCode for TailwindCSS Markup with Extension
  - Tailwind CSS IntelliSense
  - https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss 