# MiniLinks

> A URL shortener, à la Bitly, TinyURL, or Rebrandly.

MiniLinks is a very cruddy app. Users can register, login, logout, create shortened URLs, edit them, delete them, view how many times they've been visited (both uniquely and overall) and the timestamps of when they were visited as well as the date they were created.

This app was made in three days on top of other coursework, and the UI reflects that.

![MiniLinks]([demo])

## Table of contents

- [Usage](#usage)
- [Getting started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installing and running](#installing-and-running)
- [Running the tests](#running-the-tests)
- [Dependencies](#dependencies)
- [Dev Dependencies](#dev-dependencies)
- [Known issues / bugs](#known-issues-/-bugs)
- [Feature roadmap](#feature-roadmap)

## Usage

![MiniLinks](https://upload.wikimedia.org/wikipedia/commons/5/57/Bootstrap-3.1.1-screenshot-jumbotron-example.png)

The above gif demonstrates basic usage

## Getting started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

If you don't have Nodejs and npm installed, install them from [here.](https://nodejs.org/en/)

### Installing and Running

#### Windows Users

One extra step for Windows users. After this, do what everyone else does. In the root directory:

```
npm i -g node-gyp node-pre-gyp windows-build-tools chokidar
```

You can thank bcrypt for this!

#### Everyone Else

In the root directory:

```
npm install
```

And then:

```
npm run server
```

Then navigate to localhost:5050 in your browser.

## Running the tests

In the root directory:

```
npm run test
```

## Dependencies

- [Nodejs](https://nodejs.org/en/) - Javascript runtime
- [Express](https://expressjs.com/) - Framework used for API in Node
- [body-parser]() - Easily extract data from request bodies
- [bcrypt]() - Password hashing
- [cookie-session]() - Encrypted cookies to create safer sessions
- [ejs]() - Templating Engine
- [method-overide]() - Allowing more HTTP methods than POST and GET

## Dev Dependencies

- [Chai]() - Assertion library
- [Mocha]() - Testing framework
- [nodemon]() - Auto reload server for quicker debugging

## Known issues / bugs

- Severly lacking in alert functionality; the structure is there, as some alerts have been implemented (eg. successful registration) but due to time constraints, many crucial alerts are not present (eg. this email is already in use, non-matching passwords)
- The UI is destitute
- There is some client side validation, but you can still send app-breaking data to the server if you put some effort into it
- Very little testing coverage, I did the minimum required in favour of adding more features

## Feature roadmap

- Complete alert coverage, so the user always knows what's happening or what went wrong
- Complete test coverage
- Add JSDoc comments
- Make it nice to look at
- Host it on Heroku
- Attach it to a real database rather than a JSON file
- Open to suggestions, email below

Email: [bryce.j.mcmath@gmail.com](mailto:bryce.j.mcmath@gmail.com)

<!-- Markdown link & img definitions -->

[demo]: ./screenshots/demo.gif
