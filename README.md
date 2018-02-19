![cf](https://i.imgur.com/7v5ASc8.png) Lab 09: Persistence
======

## Submission Instructions
* Work in a fork of this repository
* Work in a branch on your fork
* Write all of your code in a directory named `lab-` + `<your name>` **e.g.** `lab-susan`
* Open a pull request to this repository
* Submit on canvas a question and observation, how long you spent, and a link to your pull request

## Configuration 
Configure the root of your repository with the following files and directories. Thoughtfully name and organize any additional configuration or module files.

* **README.md** - contains documentation
* **.gitignore** - contains a [robust](http://gitignore.io) `.gitignore` file 
* **.eslintrc** - contains the course linter configuratoin
* **.eslintignore** - contains the course linter ignore configuration
* **package.json** - contains npm package config
  * create a `lint` script for running eslint
  * create a `start` script for running your server
  * create a `test` script for running your tests
* **server.js** - runs your application
* **lib/** - contains helper modules
* **model/** - contains resource model(s)
* **__test__** - contains route tests

## Feature Tasks
Continue working on your vanilla REST API from yesterday. Today, you'll be refactoring several key sections of your application.  Follow the minimum requirements below *but* feel free to refactor any other areas that you deem necessary.
* All routes should be removed from your `server.js` file and contained in a separate module (ex: `route/resource-route.js`)
* All response (`res`) messages & status codes should be handled through a separate helper module (ex: `response.js`)
* Refactor the `storage.js` module to use file system persistence. This should use the `fs` module to create and read data files. For easy access, the name of the file should contain the related resource id. (ex: `2f3c44d1b9ac2b.json`)