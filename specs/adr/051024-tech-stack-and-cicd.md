# Tech Stack and CI/CD: IndexedDB, Cypress, ESLint, and JSDocs

## Context and Problem Statement

We need to decide on what tools and technologies to use. We also need to finalize our CI/CD pipeline before we can continue.

## Considered Options

* Linting: ESLint
* Code Quality: None
* Code Quality: CodeClimate
* Code Quality: Codacy
* Code Quality: Lighthouse
* Code Quality: Manual Review
* Documentation: JSDocs
* Unit Testing: Jest
* Unit Testing: Ava
* Unit Testing: Cypress
* Unit Testing: Mocha
* Unit Testing: Tape
* E2E and Component Testing: Cypress
* Database: IndexedDB

## Decision Outcome

Chosen option for linting: "ESLint", because we can use it both in our CI/CD pipeline and locally. It can also enforce style conventions and checks for errors.

Chosen option for code quality: "Manual review", because we most likely do not need any fancy tools. We are also not sure if they meet our needs. We will require multiple checks in order to merge, so checking for quality is strict. If we need need a tool to check for code quality, we can use Lighthouse.

Chosen option for documentation: "JSDocs", because it is automated, allows us to write in a format we want, and is flexible.

Chosen option for (all) testing: "Cypress", because it is good for E2E and component testing, and can also be used for unit testing. It is also seems to be convenient and easy to use.

Chosen option for data store: "IndexedDB", because it does not need any dependencies, nodejs, or any sort of backend. It may also be useful for our search feature.

<!-- This is an optional element. Feel free to remove. -->
## Validation

We will enforce the use of these tools by implementing this in our CI/CD pipeline and requiring multiple checks to merge into main.
