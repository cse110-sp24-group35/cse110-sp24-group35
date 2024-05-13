# Testing

## Context and Problem Statement
What testing libraries can we use to work well with the project? What is the required amount of testing to properly assure quality and performance?

## Decision Drivers
* Testing library compatibility

## Considered Options
* Mocha & Chai
* Cypress
* Enzyme
* Jest
* NYC

## Decision Outcome
* Use Mocha & Chai for unit testing
* Use Puppeteer on top of Mocha and Chai for E2E testing
* Use NYC for test coverage report.

## Pros and Cons of Other Options
* Cypress - Easy to setup but limited browser support. Cannot test applications that make CORS requests. Limited mobile support.
* Enzyme - Integrates with Jest and other frameworks well, but only tests React.
* Jest - Easy to setup, but very heavy bundle size and there's performance overhead for large test suites.