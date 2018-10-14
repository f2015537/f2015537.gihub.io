---
layout: post
title: You're up and running!
---
# PC-Prep-Kit

## What does this project do?  
PC Prep Kit is a web application aimed at helping the peace corps volunteers with awareness about Malaria and its prevention techniques. The application uses various interactive activities to make the process effective. The App focuses on causes, prevention and medication of Malaria.

## Why is the project useful? 
PC Prep kit helps spread awareness about Malaria. According to WHO[1], In 2015 there were around 212 million cases of malaria and 429,000 deaths, 90% of which is from Africa.  It is established that early diagnosis and prompt treatment of malaria prevents deaths. Taking simple preventive measures can also help in preventing malaria to a large extent. The Peace Corps Volunteers who travel to the countries effected with malaria can use the information proved in the application and learn about symptoms, medications and their side effects and preventive measure which help keep them safe. 

## Technologies used
The project uses 
* Node.js 8.11.2, Express framework (JavaScript)
* Angular 6 (SCSS, TypeScript, HTML)
* Mocha, Supertest, Should.js (Backend Testing)
* Jasmine, Karma (Angular Testing)
* MySQL + Sequalize ORM 
* ESLint and TSLint (Linting tools)
* Python
* Tensorflow
* Rasa_Core and Rasa_NLU



## How can users get started with contributing to the project? 
  
Anyone can find an issue in the application, the issue is not limited to bugs but also includes UI enhancements, efficient codes, improved structure, updating depreciated functions or adding more dialogues in the ChatBot Dialogue Corpus.  
  
The following procedure must be followed in order to solve an issue.    
  
* Check if the issue has already been reported, if not report the issue on Github.
* Assign the issue to yourself, if you want to solve it.  
* You can open an issue and tag it as free if you do not wish to solve it. 
* The issues marked free are open for you to solve, assign the issue to yourself before beginning the work on it. 
* Before you make a Pull request, make sure that there are no linting errors with the files you modified.

## Getting Started

#### Fork the Repository
On GitHub, navigate to the PC-Prep-Kit Repository.
In the top-right corner of the page, click Fork.

#### Clone the Repository
Now, navigate to the forked repository in your profile.
In the top-right corner of the page, you will find a green button with the text "Clone or download". Click on it.
Copy the link that appears in the popup.

Now, go to your terminal (if you are using a Linux platform) or git bash (if you are using a Windows platform) and execute this command

```
git clone URL
```

Replace URL with the copied url

or you can just,

Go to your terminal and execute this command

```
$ git clone https://github.com/YOUR_USERNAME/PC-Prep-Kit
```
Replace YOUR_USERNAME with your Github username.

### Installation

Install all dependencies in package.json file. This can be done by navigating to the cloned PC-Prep-Kit directory in the command prompt/terminal/console and running the following command:

```
$ cd PC-Prep-Kit
$ npm install
```

Edit the `settings.js` file inside the config folder with your custom API keys and database setup information.

Create a new tab in your terminal/command line and in there log in to your local MySQL account and follow the steps below:

```
CREATE DATABASE pcprepkit;
```

or if you are using a tool like phpMyAdmin to manage your database, you can setup it up there too.

#### Starting up the Bot Server

Optional. That is, only if you want to use the ChatBot. To set up this, Detailed instructions are given [here](https://github.com/systers/PC-Prep-Kit/wiki/ChatBot-Documentation).

Once the database and the bot server (optional) is setup, run the following command from the project directory.
```
$ npm start
```

Then create a new terminal or command line tab and go to the project directory and run

``` 
$ ng build --watch
```

to setup the Angular developmental server.

After the build completes, you can navigate to http://localhost:3000/ in your browser to check out the application. 

And, that's it, you are DONE. You have successfully setup the project.

The app will automatically reload if you change any of the source files.

### Testing 
#### Backend Testing
Backend Testing uses mocha, supertest and should.js, these packages are installed automatically from the package.json file and will be available after all the packages are installed by running `npm install`.  
The test file is available in test/test.js.  
To contribute to the backend testing for PC Prep Kit, you can search for APIs for which the test cases have not been written, or validity of current tests due to any API changes.   

#### Angular (Frontend) Testing
Frontend Testing uses Karma and Jasmine, these packages are installed automatically from the package.json file and will be available after all the packages are installed by running `npm install`.
All component tests are within the respective component folders and service tests are in *src/tests* folder.

Steps to run the tests:
Run `ng test` to execute the unit tests via Karma.

To contribute to the frontend testing for PC Prep Kit, you can look for files for which the test cases have not been written, or fix test cases that fail. In some tests, we have imported similar modules and components. A new common module may be formed and imported.

#### Running TSLint and ESLint

Run `ng lint` in your terminal to identify all linting errors with Angular files. 

You can also run `tslint PATH_TO_YOUR_typescript_FILE` to check for linting errors of individual files.

Run `eslint *.js; eslint **/*.js` in your terminal to identify all linting errors with Node files. 

You can also run `eslint PATH_TO_YOUR_nodejs_FILE` to check for linting errors of individual files.


#### Need more help?

[Help on using Git](https://forum.freecodecamp.org/t/wiki-git-resources/13136)

To get more help on the angular-cli use `ng --help` or go check out the [Angular-CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

Run `npm install --save PACKAGE_NAME` to install packages locally and add it to package.json file.

Or

Run `npm install -g PACKAGE_NAME` to install packages globally and use it across all node projects.

Replace PACKAGE_NAME with the actual name of the package.

Still having trouble installing npm packages. You can learn more about it  [here](https://docs.npmjs.com/getting-started).

Get help on Sequelize [here](http://docs.sequelizejs.com/).

## Where can users get help with the project?
Users can post their questions on the [Slack Channel](http://systers.io/slack-systers-opensource/) group pc-prep-kit or use the [Mailing List](http://systers.org/mailman/listinfo/systers-dev) . 

[1] [WHO - 10 facts about malaria](www.who.int/features/factfiles/malaria/en/)
