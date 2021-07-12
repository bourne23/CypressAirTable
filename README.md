## CypressWorkshop - Airtable
 A project to demonstrate/test a use case, i.e. signup and onboarding flow using Cypress 

## Prerequisites
1. Install Node JS and Setup NPM
```bash
npm install 
```
2. Install Visual Studio Code Editor or another IDE

3. If you have npm version older than npm@5.2.0, install npx to run ``cypress open``
```
npm install -g npx
```
4. Install Chrome browser 

## Running the project
Run tests by using terminal or an NPM scripts 
For headless execution:
```bash
npx cypress run ./cypress/integration/aritable/signup.spec.js
```
To open test in browser
npx cypress open ./cypress/integration/airtableSignup/sample_spec.js
```bash
npx cypress run ./cypress/integration/aritable/signup.spec.js
```

```bash
├── README.md
├── cypress
│   ├── fixtures
│   │   └── example.json
│   ├── integration
│   │   └── airtable
│   │       └── signup.spec.js
│   ├── plugins
│   │   └── index.js
│   ├── support
│   │   ├── commands.js
│   │   └── index.js
│   └── videos
│       └── aritable
│           └── signup.spec.js.mp4
├── cypress.json
├── package-lock.json
└── package.json
```
## Test requirements
Prerequisites:
Go through the signup flow from airtable.com and observe each step of the onboarding flow
If you are unfamiliar Cypress, watch quick tutorials to see if there is a preference for one over the other
Use cypress-testing-library if possible.
Sign up for a user account on Airtable
Invite an additional user (see: Adding a collaborator)

Instructions:
For this exercise, you will design a test that will successfully create an account and take you through the onboarding process, either as a standalone user or an invited user
Verify that you have created a new base
Share the base with a collaborator by using “Invite by email” flow
Set the permission level as “Editor”
Verify that the newly collaborated user email is displayed under “Base Collaborators”
Verify that the collaborator has “Editor” role displayed under “Base Collaborators”

Suggestions:
You can submit this as a single test case and verify it can run through fully and succeed
Include a README.md file on setting up and running the tes