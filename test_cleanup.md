Important terms and ideas:

1. Cleanup code: Code that is used to undo or clean up any side effects or changes made during the execution of tests.
2. Mocking: Creating a simulated or fake version of a function or object to isolate the code being tested and control its behavior.
3. Sandbox: A controlled environment where the code being tested is isolated and its side effects are contained.
4. afterEach: A hook provided by Jasmine that runs after each individual test, allowing you to perform cleanup or reset operations.
5. beforeEach: A hook provided by Jasmine that runs before each individual test, allowing you to set up initial conditions or states.
6. beforeAll: A hook provided by Jasmine that runs once before all the tests, typically used for setup tasks that need to be done once.
7. afterAll: A hook provided by Jasmine that runs once after all the tests, typically used for cleanup tasks that need to be done once.
8. Matcher: A function provided by Jasmine that performs a comparison between an actual value and an expected value to determine the test result.

Code snippets:

1. Using afterEach to perform cleanup:
```javascript
describe('submitForm tests', function() {
  afterEach(function() {
    // Reset input value and usernames array
    input.value = '';
    usernames = [];
  });

  it('saves input val to usernames array', function() {
    // Test case code
  });
});
```

2. Using beforeEach to set initial conditions:
```javascript
describe('submitForm tests', function() {
  beforeEach(() => {
    console.log('BEFORE!');
    // Other setup code
  });

  it('saves input val to usernames array', function() {
    // Test case code
  });
});
```

3. Using beforeAll and afterAll:
```javascript
describe('submitForm tests', function() {
  beforeAll(() => {
    console.log('BEFORE ALL');
    // Construct test database or perform setup tasks
  });

  afterAll(() => {
    console.log('AFTER ALL');
    // Remove test database or perform cleanup tasks
  });

  it('saves input val to usernames array', function() {
    // Test case code
  });
});
```

These code snippets demonstrate the usage of hooks provided by Jasmine, such as afterEach, beforeEach, beforeAll, and afterAll, to perform cleanup, set up initial conditions, or simulate specific states for testing. These hooks help ensure that each test is executed in a controlled and isolated manner.