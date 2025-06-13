# evercycle-redirect
This is to fix Domain Issue for MXToolbox


# Evercycle.io Root Domain Redirect Service

This repository contains a simple redirect service for the root domain `evercycle.io` to resolve MXToolbox validation issues.

## Problem
- Webflow blocks automated crawlers (including MXToolbox) with 403 errors
- This creates domain reputation issues affecting email deliverability
- Customer firewalls reject emails from domains flagged by monitoring tools

## Solution
- Host root domain (`evercycle.io`) on Netlify
- Provides proper 200 OK responses to validation tools
- Redirects all traffic to `https://www.evercycle.io` (hosted on Webflow)

## Deployment
1. Connect this repository to Netlify
2. Update DNS for `evercycle.io` to point to Netlify
3. Keep `www.evercycle.io` pointing to Webflow

## Files
- `public/index.html` - Simple redirect page
- `netlify.toml` - Netlify configuration with redirects and security headers

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
















