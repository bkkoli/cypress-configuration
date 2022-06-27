# How to configure Cypress in Nuxt js ?
- [reference](https://docs.cypress.io/guides/component-testing/component-framework-configuration#Nuxt)

## 1. Install Cypress
```bash
npm i -D cypress
```

## 2. Modify your package.json
```diff
{
    "scripts": {
-        "test": "echo \"Error: no test specified\" && exit 1"
+        "test": "./node_modules/.bin/cypress open"
    }
}
```

## 3. Run Cypress server
```bash
npm run test
```