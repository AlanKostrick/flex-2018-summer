# Delightful JavaScript Testing with Jest

There are several frameworks utilized today for testing your JavaScript. Each comes with its own set of features and developer preferences, but we enjoy Jest because of its lightweight and conventional setup. Out of the box it comes with very descriptive test results printed directly to your console. 

If a testing environment is complicated to set up, developers will look at it as a burden instead of a tool. Being able to get up and running quickly and seamlessly will encourage more tests! 

Jest is used by Facebook to test their React applications.


## Installing Node

- [This needs to be done first](https://nodejs.org/en/download/)
- Verify installation: `node-v`
- Verify node package manager: `npm -v`

## Install Jest in your project

- `mkdir jest-api-demo`
- `cd jest-api-demo`
- `npm init -y` will create a package.json file
- `npm i -D jest` installs the Jest Dependency
- open up the package.json file and where it says testscript write jest like this: `testscript: "jest"`

## Install Axios (to use instead of fetch)

- Useful for Asunchronous data
- `npm i axios`

## Create a basic function file to test

- `functions.js` 
  - Place this code at the top of the file: `const axios = require('axios');`
  - Place this code at the bottom of the file: `module.exports:functions`
- `functions.test.js` and place this code inside of the file: `const functions=require('./functions);`

## Let's run a basic test to make sure we are wired up 

In `functions.js`

```
const functions = {
	add: (num1, num2) => num1 + num2
  };
```

In `functions.test.js`
```
test('Adds 2 + 2 to equal 4', () =>{
	expect(functions.add(2,2)).toBe(4);
});
```
