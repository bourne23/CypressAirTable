## CypressWorkshop - Airtable
 This repo contains an example project with the a test written in Cypress.

## Prerequisites
1. You have Node JS installed and NPM set up, and version no later than npm@5.2.0
```bash
npm install 
```
2. You have Visual Studio Code editor 
3. You have Chrome browser installed

## Running the project
Run tests by using terminal or an NPM scripts 
For headless execution:
```bash
npx cypress run ./cypress/integration/aritable/signup.spec.js
```
To open test in browser:
```bash
npx cypress open ./cypress/integration/airtableSignup/sample_spec.js
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
```bash
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
Include a README.md file on setting up and running the test
```
