### How Angular Unit test case Flow?

- `The Angular testing package includes two utilities called` **TestBed and async**
- `TestBed is the main Angular utility package.`
- `The describe container contains different blocks (it, beforeEach, xit, etc.).` 
- **beforeEach** `runs before any other block. Other blocks do not depend on each other to run.`

`The Angular CLI downloads and installs everything you need to test an Angular application with the Jasmine test framework. The ng test command builds the application in watch mode, and launches the Karma test runner.`

![image](https://user-images.githubusercontent.com/53125546/216266354-368a9e24-168c-4187-8683-bf8c70d2c2af.png)

`There will be multiple things you will notice from the above code snippet, What each of this does is explained below:`

- **We use a “describe” to start our test and we give the name of component that we are testing inside it.**

- **The beforeEach tells the Karma test runner to run this code before every test in the test suit, i.e it().**
- **Inside the beforeEach, we have TestBed.ConfigureTestingModule. What TestBed does is, It sets up the configurations and initialises the environment suitable for our test. ConfigureTestingModule sets up the module that allows us to test our component. We can say that it creates a module for our test environment and have Declarations, Imports, and Providers inside it.**

- **We declare the component that we test inside the Declarations array. We have to include those of other components If our component of interest has a dependency on them.**

- **In the Provider array, we override the actual service with our spy that we created using Jasmine. Other services that are injected into our component through the constructor are provided directly in this array if we don’t want to spy on them.**
