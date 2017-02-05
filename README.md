# Using Requestly in Visualforce Development Workflow
It's time that front-end development workflow on Salesforce gets an efficiency boost. 

If you've developed any front-end assets on localhost, you may know how incredible it is to use tooling like [Gulp](), [Grunt](), and most recently [Webpack](); updating a function in your JS or changing a style in your CSS causes the page to reload, and you continue forward with development. This same workflow is possible with your Visualforce development workflow by using a static resource bundle, a Chrome extension called [Requestly](), and your task runner of choice (in this case, [Webpack]()).

## Prerequisites
In order to benefit from developing and serving your front-end components on localhost, you'll need to have a few things set up first.

1. `cd` to your project's root folder
1. `npm init` and `npm install webpack-dev-server --save-dev`
1. Ensure that your Visualforce page uses a static resource to reference your JS and CSS

## Setting Up Webpack
The first step is creating a Webpack config file that watches for changes to your local JS and CSS files. There are plenty of complex workflows that Webpack can do, but we'll primarily leverage its ability to track your JS and CSS file changes and serve them to localhost.

```js
```

Run `webpack-dev-server --content-base resource-bundles/RequestlyDemo.resource --https`

IMAGE: check out the URL to your CSS and JS files
![]()

## Setting Up Requestly


IMAGE: JS console to inspect sources
![]()

IMAGE: creating a Requestly redirect rule
![]()