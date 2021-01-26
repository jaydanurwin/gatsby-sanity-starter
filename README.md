# Gatsby Sanity Starter

## What you have

- A blazing fast blog with [Gatsby.js](https://gatsbyjs.org)
- Structured content using [Sanity.io](https://www.sanity.io)
- (Optional) Global deployment on [Netlify](https://netlify.com)

## Quick start

1. Clone this repository
2. `cd sanity`
3. `npm install -g @sanity/cli`
4. `sanity init` and follow the prompts (you will need to create a Sanity account if you haven't already)
5. `npm run graphql-deploy`
6. `cd ..` to navigate back to the root folder
5. `npm install` in the project's root folder
6. `npm run dev` to start the studio and frontend locally
   - Your studio should be running on [http://localhost:3333](http://localhost:3333)
   - Your frontend should be running on [http://localhost:8000](http://localhost:8000)
7. Open [http://localhost:3333](http://localhost:3333) and copy the project ID from the Project info section
8. Navigate to the client-config.js file in the gatsby directory
9. Replace the project ID with your Project ID
10. `npm run build` to build to production locally

## Enable real-time content preview on development

1. Go to your [project’s API settings on manage.sanity.io](https://manage.sanity.io/projects/adxlh59f/settings/api) and create a token with read rights.
2. Rename `.env.development.template` to `.env.development` and paste in the token: `SANITY_READ_TOKEN="yourTokenHere"`.
3. Restart the development server (`ctrl + C` and `npm run dev`).

If you want to turn off preview you can set `watchMode: false` in gatsby-config.js. If you just want to preview published changes you can set `overlayDrafts: false` in gatsby-config.js.

## Deploy changes

Netlify automatically deploys new changes commited to master on GitHub. If you want to change deployment branch, do so in [build & deploy settings on Netlify](https://www.netlify.com/docs/continuous-deployment/#branches-deploys).

## Stuck? Get help

[![Slack Community Button](https://slack.sanity.io/badge.svg)](https://slack.sanity.io/)

Join [Sanity’s developer community](https://slack.sanity.io) or ping us [on twitter](https://twitter.com/sanity_io).
# gatsby-sanity-starter