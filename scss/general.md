# SCSS

## Setting up the developement enviroment

It is important to know that there are two enviroment and the Developer side with all it's tools and packages, and the client/server side, meaning the version that will be deployed.

- Developer side = src;
- Deployed version = dist;

### =\> _Developement: Tools and packages_

In order to setup the developer side we need to access the packages from **node package manager**:

1.  `npm init` or `npm init -y` (this last one is for doing everything automatically);

> This command initiate the process of creating a package.json file where it stored information regarding the project, the developer, project dependencies and uselfull scripts to assist in the development proccess.

2.  `npm i --save-dev gh-pages sass npm-run-all liver-server`

> Installing dependencies and packages that will be used in the development side:
>
> - gh-pages
> - sass
> - nmp-run-all
> - live-server
>   Obs.:
>   1- The `--save-dev part` of the command is to specify that the following commands are developer tools.
>   2- The `i` after `npm` stands for install

3.  Adding the following scripts to the package.json file:

"scripts": {
"start": "run-p watch watch:styles",
"build": "run-s clean clean:styles build:styles copy",
"deploy": "run-s build publish",
"build:styles": "sass src/scss:src/styles",
"watch": "live-server src",
"watch:styles": "sass src/scss:src/styles --watch",
"clean": "rm -rf dist",
"clean:styles": "rm -rf src/styles",
"copy": "mkdir dist && rsync -avr --exclude=\"/scss\" src/ dist",
"publish": "gh-pages -d dist"
},

4- `npm start`

> This command run the live-server and sass in watch mode

## =\> _Deployment: Commands_

- `npm run build`

> Transpile and copy the Sass files as well as relevant files from src to dist to prepare your website for deployment.

- `npm run deploy`

> Prepare your code to be deployed to Githob Pages:This script creats a 'gh-pages' branch and publishes the dist folder. For this to work, make sure you already have a remote repository on github.

---

```
New workflow
```

1.  Create the repository for the project on github;
2.  Initialize git;
3.  Initialize npm;
4.  configure the package.json file;
5.  Create the src directory and the scss directory inside of root directory;
6.  Inside the src directory create the index.html file, and inside the scss directory create the main.scss file;
7.  Use the npm start command to start the live server and the watch packages;
8.  Work away and create the project!
9.  Git! `git add . && git commit -m "some pertinent comment"`, after that `git push origin main`;
10. After updating the develper tools we need the deployable version, with: `npm run build`;
11. The final version is to update the gh-page with the command: `npm run deploy`.

---

## Coding with Sass

declarative and imperative variables
