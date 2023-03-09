# React Webapp using Webpack and Tailwind

To start a react app

    npx create-react-app appname

Command to install the rest of the required packages and add them as dev-dependencies

    npm install -D tailwindcss postcss autoprefixer
Command to generate <b>postcss.config.js</b> and <b>tailwind.config.js</b>

    npx tailwindcss init -p
Compiling a css file to an equivalent browser-understandable css file:-

    npx tailwindcss -i ./public/styles/input.css -o ./public/styles/tailwind.css
This setup will traverse through all the files and folders listed in the <b>content</b> of <b>tailwind.config.js</b> and load only those Tailwind CSS classes which are currently used by our app

All the rest of the dependencies are listed in the <b>package.json</b> file

## Key difference between npm and npx
npm is used to install and remove packages <br>
npm is used to execute a package

## Building
Build the page using homepage:"." in <b>Package.json</b>
Then change the homepage according to the url structure
## Running Tests
The tests folder contains unit-tests written in mocha and chai. To run tests, use the command

    npm test

    > calculatorz@1.2.3 test
    > npx mocha src/tests.mjs

        Determinant
            ✔ should return -168

        Complex Determinant
            ✔ should return -393+225i


        2 passing (11ms)
