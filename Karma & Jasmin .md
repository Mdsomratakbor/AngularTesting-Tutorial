### What is Karma?
`Karma is a direct product of the AngularJS team from struggling to test their own framework features with existing tools. As a result of this, they made Karma and have transitioned it to Angular as the default test runner for applications created with the Angular CLI.`

`In addition to playing nicely with Angular, it also provides flexibility for you to tailor Karma to your workflow. This includes the option to test your code on various browsers and devices such as phones, tablets, and even a PS3 like the YouTube team.`

`Karma also provides you options to replace Jasmine with other testing frameworks such as Mocha and QUnit or integrate with various continuous integration services like Jenkins, TravisCI, or CircleCI.`

`Unless you add some additional configuration your typical interaction with Karma will be to run ng test in a terminal window.`

**Spectacular Test Runner for JavaScript. Karma is not a testing framework, nor an assertion library. Karma just launches a HTTP server, and generates the test runner HTML file you probably already know from your favourite testing framework. So for testing purposes you can use pretty much anything you like. Jasmine can be classified as a tool in the "Javascript Testing Framework" category, while Karma is grouped under "Browser Testing". "Can also be used for tdd " is the primary reason why developers consider Jasmine over the competitors, whereas "Test Runner" was stated as the key factor in picking Karma.**


### What is Jasmine?

`Jasmine is a behavior-driven development framework for testing JavaScript code that plays very well with Karma. Similar to Karma, it’s also the recommended testing framework within the Angular documentation as it’s setup for you with the Angular CLI. Jasmine is also dependency free and doesn’t require a DOM.`

`As far as features go, I love that Jasmine has almost everything I need for testing built into it. The most notable example would be spies. A spy allows us to “spy” on a function and track attributes about it such as whether or not it was called, how many times it was called, and with which arguments it was called. With a framework like Mocha, spies are not built-in and would require pairing it with a separate library like Sinon.js.`

`The good news is that the switching costs between testing frameworks is relatively low with differences in syntax as small as Jasmine’s toEqual() and Mocha’s to.equal().`
