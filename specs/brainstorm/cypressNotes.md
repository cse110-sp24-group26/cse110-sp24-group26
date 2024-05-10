# _Cypress Unit Testing_ #

https://www.cypress.io/

Cypress is a testing tool intended __specifically for for web development__. The main feature is a __visual testing application__
that is easy to use, and very informative. The application displays your tests __as they run__, and displays your website
__as if a user were actually interacting with it__. When you launch the program from the command line, cypress automatically
launches in the selected browser (I had an option of 3, including chrome). From there, your tests run, with live repsonses
from your website. Cypress interacts with your website __the same way a user would__, and the syntax for writing tests
__works seemlessly with your DOM__.

- [Set up tests](https://docs.cypress.io/guides/overview/why-cypress#Writing-tests)  
  _There are no servers, drivers, or any other dependencies to install or configure._  
  ```
  cd <your Repo>
  ```
  ```
  npm init
   ```
  ```
  npm install cypress --save-dev
  ```
  ```
  npx cypress open
  ```
- [Write tests](https://docs.cypress.io/guides/overview/why-cypress#Writing-tests)
  - Once you've configured e2e: (or whatever you choose, I haven't experimented with anything else yet)
  - Write your tests.
  - General format looks like:
    ```
    describe('TestSuiteName', () => {

      beforeEach(() => {
        cy.visit('<your Website')
      })
    
      it('test1', () => {
        cy.get('someElement')
          .select('someValue')  //if it's a selector element
      })
      
      it('test2', () => {
          //do stuff
          cy.wait(2000)
          //do more stuff
      })
    
      it('test3', () => {
        cy.get('someButton')
          .click()
      })
    })
    ```
  - Also obviously includes simple ways to do assertions and check values and stuff, I haven't experimented yet.
- [Run tests](https://docs.cypress.io/guides/overview/why-cypress#Running-tests)
  ```
  npx cypress open
  ```
  - Use very intuitive ui in app that automatically opens. (It's pretty sweet)
- [Debug Tests](https://docs.cypress.io/guides/overview/why-cypress#Debugging-tests)
  I haven't looked into this yet, but it seems like it needs external dependencies, and I feel like debugging your tests
  is something that only a psycopath would do. (Testing web apps is already pretty psychotic in the first place ☻) 





## Writing Tests For Lab 5 ##

To implement this:
1. Make sure you have node.js installed
2. Go to directory
3. run `npm install cypress --save-dev`
4. Run `npm init`
5. Run `npx cypress open`
6. Choose e2e testing
7. Quit
8. Paste the following code into cypress\e2e\spec.cy.js (or whatever it created for you to write tests in)
9. Run `npx cypress open`
10. Select the test
11. The test (which I was able to write in about 20 mins wihtout having ever used cypress) should test all functionalities of the .expose part of the lab. (change horn, change volume, play sound)
12. HMU for any issues. (Ekin C.)
```
describe('test', () => {

  beforeEach(() => {
    cy.visit('https://<insert your pages link here>')
  })
  it('play party', () => {
    cy.get('#volume')
      .invoke('val', 100)
      .trigger('input')
    cy.get('#horn-select')
      .select('party-horn')
    cy.get('button')
      .click()
      cy.wait(2000)
  })
  
  it('play car and lower volume', () => {
    cy.get('#volume')
      .invoke('val', 25)
      .trigger('input')
    cy.get('#horn-select')
      .select('car-horn')
    cy.get('button')
      .click()
      cy.wait(2000)
  })

  it('play air', () => {
    cy.get('#volume')
      .invoke('val', 1)
      .trigger('input')
    cy.get('#horn-select')
      .select('air-horn')
    cy.get('button')
      .click()
      cy.wait(5000)
  })
})
```
__Note:__ This assumes your volume slider (range element) uses an `'input'` listener.  
__Note:__ Replace `<insert your pages link here>` with your pages link to the ".expose" part.
