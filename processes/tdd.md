# My TDD process
1. Using your [domain] model, write simplest, first feature test for the first user story, using a REPL, to understand how you might interact with the program and the classes, methods, etc you know about so far. Watch the fail (RED step).

2. (This feature test could be automated in your test suite, or added to a test helper so the set up activies required don't have to be repeated manually for each subsequent test. This would likely be part of a later refactor).

3. Write a minimum first unit test, with the aim being to replicate the error that the feature test is producing (RED step).

4. (These early tests can be scaffold tests to start building out the file and ```class``` structure).

5. Write the minimum code to pass the tests - follow the error messages when running the test suite, and fix only what the error is suggesting, i.e.

  * If error reads ```NameError : uninstantiated Class``` or similar, create the class

  * if error reads ```NameError : undefined Method``` or similar, create the method

  * if error reads ```ArgumentError : expected 0 received 1``` r similar, add the necesary number of arguments

6. Follow the next error and keep repeating until the test passes (GREEN step).

7. Refactor code and tests as necessary (REFACTOR step)

8. Regularly run irb or features tests to check expected behaviour.

9. Repeat the process for next requirement.
