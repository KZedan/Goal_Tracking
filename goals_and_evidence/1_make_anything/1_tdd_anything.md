# I can make anything
## I can TDD anything
### Reflect: What does it mean to be able to TDD anything?

The ability to take requirements (user stories) and the behavioural descriptions they provide to guide first the test I write, and then the code I write to pass that test.

To be able to test-drive anything means that I am comfortable and confident to take any problem and follow a structured process so that each test should be the simplest next step, and each piece of code written should be the simplest to pass that test and nothing more. I am guided by the behaviour required via a user-focused feature test and the subsequent, related unit tests.

Following this ```red```, ```green``` and then ```refactor``` cycle ensures clean, minimal and well-designed code, with maximum test coverage.

### Process
Overview

* Break out the objects and messages from the user story, and create a table highlighting which messages you expect to be passed to which objects.

* Write a feature test for the user story (how a user may expect to interact with the class(es) and method(s) in the story) - this can be in a repl, or later in the development process, in an automated feature test file.

* Use the first feature test failure to guide the first unit test.

* Use the first unit test failure to guide the first (and absolute simplest) code implementation to pass both tests.

* Repeat.

detail

My [process](https://github.com/KZedan/Goal_Tracking/blob/master/processes/tdd.md) in detail, for test_driving anything.



### Plan: List evidence you aim to collect that would together show you have credibly achieved this goal
