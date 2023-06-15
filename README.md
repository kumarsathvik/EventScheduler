# React Event Scheduler App

<!-- [![](https://img.shields.io/github/workflow/status/AhmedAlatawi/react-event-scheduler/Build%20and%20Test)](https://github.com/AhmedAlatawi/react-event-scheduler/actions/workflows/main.yml) -->
[![Depfu](https://badges.depfu.com/badges/e9fb7e6c5e5b18f9b1dbf2c05736f034/status.svg)](https://depfu.com)
[![Depfu](https://badges.depfu.com/badges/e9fb7e6c5e5b18f9b1dbf2c05736f034/overview.svg)](https://depfu.com/github/AhmedAlatawi/react-event-scheduler?project_id=35359)
[![Depfu](https://badges.depfu.com/badges/e9fb7e6c5e5b18f9b1dbf2c05736f034/count.svg)](https://depfu.com/github/AhmedAlatawi/react-event-scheduler?project_id=35359)
[![License: MIT](https://img.shields.io/github/license/AhmedAlatawi/react-event-scheduler)](https://github.com/AhmedAlatawi/react-event-scheduler/blob/master/LICENSE)

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

![](./images/react-event-pic.gif)

Event Scheduler is a React app that allows users to create events. An event can be anything, such as a sport event, team meeting, party announcement, personal advertisement, etc. An event consists of title, start and end date/time, and description. Events can also be shared on FB or Twitter.
All events are public by default (visible to everyone). They can also be private (only visible to you) by checking the private checkbox.

### [Demo](https://react-event-scheduler.vercel.app/) :movie_camera:

## Tech Stack

### Frontend

- React (react hooks)
- Typescript
- Bootstrap/react-bootstrap
- Styled components
- Apollo client
- JS cookie

### Backend

- NodeJS with Express
- Typescript
- Apollo server express
- JSON web token
- MongoDB with mongoose

### This project implements Apollo advanced caching mechanisms for better performance (posting or fetching data from the serve is only performed when needed)

---

Note that `graphql` schemas are generated using [GraphQL Code Generator](https://www.graphql-code-generator.com/docs/getting-started). This means that if you make any changes to the schema (server/graphql/schema/index.ts), make sure that the `.graphql` files in the frontend are also updated accordingly. Next, run `yarn codegen` to re-generate the gueries and mutations on the frontend (Note: before you do this, make sure the server is up and running by either running `yarn start` or `yarn start:server`)

[GraphQL Playground](https://github.com/graphql/graphql-playground) is a powerful GraphQL IDE enabling better (local) development workflows. It helps test your schemas locally. See image below:

![](./images/graphql_playground.PNG)

## Run app locally

> Make sure MongoDB is up and running

In the project directory, run `yarn`, then:

### `yarn start`

Runs the backend and frontend apps simultaneously in the development mode.\

> Or if you prefer running the apps separately by running `start:web` and `start:server` in separate terminals.

Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make changes.\
You will also see any lint errors in the console.

## Current functionality

- User signup and login
- Create, update and delete events
- Search & pagination
- Make events as private (only visible to creators)
- Session expiry warning (displayed when being idle for 3 minutes after logging in)
- Share events with family & friends on Facebook and Twitter

### Coming soon

- User profile
- Admin tab & profile

## Run unit tests

coming soon...

## Run E2E tests

coming soon...

