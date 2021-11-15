**Tailwind Setup Guide**

1) To install Tailwindcss use this command - npm install tailwindcss

2) create src and public folder then import tailwindcss components,utilities and base in src /styles.css

3) To create public /style.css file, you have to go to package.json and change the scripts to "build-css": "tailwindcss build src/styles.css -o public/styles.css" 

4) To build /styles.css in public folder use this command "npm run build-css" which takes /styles.css file from src folder 

so, you are ready to use Tailwindcss in your project!

**Whenever you make any changes to /style.css file you need to run build**

**Config file**
if you want to have your own classes like you customized one's, then you need to get "tailwind.config.js" which yon create by using command "npx tailwindcss init --full" then again run the build using command "npm run build-css"

but creating our own classes in the main config file would be a mess so instead rename that config file to config-default and now run the command "npx tailwindcss init" note this time we are not using '--full' because we don't want those already made classes in this file so that we can write our own classes in and extend.
