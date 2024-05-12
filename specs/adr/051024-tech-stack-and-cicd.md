---
# Configuration for the Jekyll template "Just the Docs"
parent: Decisions
nav_order: 100
title: ADR Template

# These are optional elements. Feel free to remove any of them.
# status: {proposed | rejected | accepted | deprecated | … | superseded by [ADR-0005](0005-example.md)}
# date: {YYYY-MM-DD when the decision was last updated}
# deciders: {list everyone involved in the decision}
# consulted: {list everyone whose opinions are sought (typically subject-matter experts); and with whom there is a two-way communication}
# informed: {list everyone who is kept up-to-date on progress; and with whom there is a one-way communication}
---
<!-- we need to disable MD025, because we use the different heading "ADR Template" in the homepage (see above) than it is foreseen in the template -->
<!-- markdownlint-disable-next-line MD025 -->
# Tech Stack and CI/DC: IndexedDB, Cypress, ESLint. and JSDocs

## Context and Problem Statement

We need to decide on what tools and technologies to use. We also need to finalize out CI/CD pipeline.

## Considered Options

* Linting: ESLint
* Code Quality: None
* Code Quality: CodeClimate
* Code Quality: Codacity
* Code Quality: Lighthouse
* Code Quality: Manual Review
* Documentation: JSDocs
* Unit Testing: Jest
* Unit Testing: Ava
* Unit Testing: Cypress
* Unit Testing: Mocha
* Unit Testing: Tape
* E2E and Component Testing: Cypress

## Decision Outcome

Chosen option for linting: "ESLint", because we can use it both in CI/CD and locally. It can also enforce style convenstions and checks for errors.

Chosen option for code quality: "Manual review", because we most likely do not need any fancy tools for it. We are also not sure if the tools meet our needs. If we need to check for code quality, we can use Lighthouse.

Chosen option for documentation: "JSDocs", because it is automated, allows us to write as much documentation as we want, and is flexible.

Chosen option for (all) testing: "Cypress", because it is good for E2E and component testing, and can also be used for unit testing. It also has an intersting interface and seems easy to use. 


<!-- This is an optional element. Feel free to remove. -->
## Validation

We will enforce this by implementing this in our CI/CD pipeline. 
