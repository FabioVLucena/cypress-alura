# cypress-alura
npm init

npm i cypress --save -include=dev

https://alura-fotos.herokuapp.com

npm run test

describe
contains
get
should('contain')

npx cypress run

npm i -D mochawesome

    "reporter": "mochawesome",
    "reporterOptions": {
    "reportDir": "cypress/report/mochawesome-report",
    "overwrite": true,
    "html": true,
    "json": false,
    "timestamp": "mmddyyyy_HHMMss"
    }     

npx cypress run --reporter mochawesome

Cypress.Commands.add('login', (nome, senha) => {
    cy.get('input[formcontrolname="userName"]').type(nome);
    cy.get('input[formcontrolname="password"]').type(senha, {log: false});
    cy.get('button[type="submit"]').click();
})
