

https://apibeta.shippable.com/projects/53bf743855a71a2200f19dee/badge/master

## Selenium tests with Node.JS! 
Basic "Hello World" example of Selenium browser tests that run on [Shippable.com](shippable.com). Uses the `nightwatch` `npm` module and Node.JS.
Jun 10
### How to run selenium tests locally?

First, execute the bash script to download and run a local Selenium server.

```
./selenium.sh
```

Then, use `npm` to run the test script. This will start the Node.JS web server so that it can be reached by the Selenium tests.
After the web server is running it will start `nightwatch` to run the Selenium tests.

```
npm test
```

### Example output:

```
» npm test

> sample_node_selenium@0.0.0 test /Users/roland/Source/shippable/sample_nodejs_selenium
> node ./server.js & ./node_modules/.bin/nightwatch

Server running at http://127.0.0.1:1337/

[ sample_test module ]

Running:  test sample
Stopping server running at http://127.0.0.1:1337
✔  Element <body> was visible after 69 milliseconds.
✔  Testing if element <body> contains text: "Hello World".
OK. 2 assertions passed. (2813 ms)
```
