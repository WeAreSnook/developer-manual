# Test driven development (TDD)

## Tools

### RSpec

For Ruby/Ruby on Rails projects we use [rspec](https://github.com/rspec/rspec)/[rspec-rails](https://github.com/rspec/rspec-rails).

We use the best-practices outlined in [Better Specs](https://www.betterspecs.org/) for our automated tests.

### Jest

For JavaScript projects we use [jest](https://jestjs.io/) as our test runner.

#### Testing React

If we're working with React then we recommend using [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/). This encourages you to focus on testing the behaviour of your components and views from the perspective of the user.

## Methodology

For developers new to test driven development it can be a steep learning curve.

When written well, automated tests allow us to change the underlying implementation without affecting behaviour. So the most important principle for software testing is:

> Test behaviour not implementation

### Software testing design patterns

There are a number of software testing design patterns that apply across languages and frameworks.

Being familiar with them design will help build your intuition of how to approach software testing.

1. [Four-phase test](https://thoughtbot.com/blog/four-phase-test)
2. [Arrange, Act, Assert](http://wiki.c2.com/?ArrangeActAssert)
3. [Given, When, Then](https://martinfowler.com/bliki/GivenWhenThen.html)

Below is a composite of the design patterns in the order shown above.

#### Setup / Arrange / Given

Our tests should be deterministic. We should be able to run them repeatably and get predictable results.

First we set our system to a particular starting state for our test. This might involve setting up a test database, creating test data or initialising mock objects.

#### Exercise / Act / When

This is where we carry out the action we are testing. This might be calling a method, interacting with a user interface or rendering a component.

#### Verify / Assert / Then

Then we test the output or resulting state of our system is what we expected. Most test frameworks provide `matchers` to help do this.

#### Teardown

The teardown phase is defined in the Four-phase test pattern. This step usually involves clearing up after ourselves. For example clearing the database or resetting the system to a base state.
