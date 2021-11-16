**Tailwind Setup Guide**

**STEPS TO INSTALL TAILWINDCSS IN YOUR PROJECT**

To generate package.json file you have to use command 'npm init -y'

Now install tailwindcss by using npm install tailwindcss

Then create a src and public folder with creating /styles.css in both the folders because what we are going to do now is, we are going to create /styles.css file in public folder with the use of /styles.css file which is in src folder

first include tailwind directives in src/styles.css : @tailwind base;
                                                      @tailwind components;
                                                      @tailwind utilities;

edit the script of package.json to "build-css": "tailwindcss build src/styles.css -o public/styles.css"

now what you have to do is run the build by command npm run build-css

**Whenever you make any changes to /style.css file you need to run build**

**Config file**
if you want to have your own classes like you customized one's, then you need to get "tailwind.config.js" which yon create by using command "npx tailwindcss init --full" then again run the build using command "npm run build-css"

but creating our own classes in the main config file would be a mess so instead rename that config file to config-default and now run the command "npx tailwindcss init" note this time we are not using '--full' because we don't want those already made classes in this file so that we can write our own classes in and extend.
