# full-stack-challenge

For testing full-stack fundamentals

## Goal of exercise

The goal of this exercise is to see whether you can start a project from scratch and build a simple web application. We are not looking for a production-ready application, but we are looking for a well-structured application that demonstrates your understanding of full-stack fundamentals.

### What you will build

The application lets the user choose different companies they want to research in order to learn if the company is a potential target account that the user's company can sell to.

The home page will contain a list / table of all the research configurations the user has created. For each configuration, there should be high level meta data about the research configuration displayed as well as a menu to edit or delete the configuration. At the top of the page there should be a call to action button that says "Create research configuration". Clicking this button will let the user create a "research configuration". This should be presented to the user as a stepper / wizard component that contains 3 steps.

- *Step 1*
  - The user can define a list of companies they want to research. The user can add and remove companies from the list. A company should consist of a name and a website url. They must define at least 1 company to continue to the next step.
- *Step 2*
  - The user can now define multiple questions they want to ask about the companies. A question should simply be an input text field. The user must define at least 1 question to continue to the next step.
- *Step 3*
  - The user can select multiple items from a dropdown of which data sources they want to check for the answers to these questions. Dropdown options can include sources such as LinkedIn, Crunchbase, etc (feel free to add your own items). The user must select at least 1 data source to be able to submit the research configuration to the backend.

To summarize, please implement the functionality for fetching multiple configurations, creating a new configuration, updating an existing configuration, and deleting a configuration.

### Things to note

- Create a simple backend server that exposes an API. Feel free to use any server framework you are comfortable with - we recommend Fastify, Express, or Koa.
- Create a basic frontend react application using any frontend component library of your choice. We recommend Mantine, Chakra, or Material UI.
- Backend and frontend are separate applications - please do not reference any code between the two. Shared code (functions, types, etc.) should be in the lib folder. Please use [ts-rest](<https://www.npmjs.com/package/@ts-rest/core>) to create a "contract" between the frontend and backend.
- You can use any database you want or you can even mock a database by reading and writing from/to JSON files.
- You can use any libraries you want, but please do not use a starter kit or boilerplate.
- Only use TypeScript!
