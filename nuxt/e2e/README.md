# End To End Test

- [reference](https://docs.cypress.io/guides/end-to-end-testing/writing-your-first-end-to-end-test#Add-a-test-file)

## 1. Add test files in e2e directory

- Your test file name must end with .cy.js

- example.cy.js

```js
describe('The Home Page', () => {
  it('successfully loads', () => {
    cy.visit('http://localhost:8080') // change URL to match your dev URL
  })
})
```

## 2. Configure Cypress

- [reference](https://docs.cypress.io/guides/references/configuration)

Cypress Configuration is defined in **cypress.config.js** file.

Examples of setting Cypress are as follows.

```js
const { defineConfig } = require('cypress')

module.exports = defineConfig({
  e2e: {
    baseUrl: 'http://localhost:8080', // change URL to match your dev server URL
  },
})
```

```js
describe('The Home Page', () => {
  it('successfully loads', () => {
    cy.visit('/') // You can visit the url which is configured in cypress.config.js file
  })
})
```

## ※ Use the Cypress Chrome Recorder

- [yotube](https://www.youtube.com/watch?v=-RJuZrq-wOk&t=150s&ab_channel=Cypress.io)
- [chrome-recorder](https://developer.chrome.com/docs/devtools/recorder/#selector)
