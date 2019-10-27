<p align="center"><a href="https://gridsome-starter-bootstrap.loke.dev"><img alt="logo" width="200" src="https://gridsome-starter-bootstrap.loke.dev/logo.png" /></a></p>

[![Netlify Status](https://api.netlify.com/api/v1/badges/70d2a5fc-0609-467a-885e-bf9518118042/deploy-status)](https://app.netlify.com/sites/gridsome-starter-bootstrap/deploys)
[![Greenkeeper badge](https://badges.greenkeeper.io/LokeCarlsson/gridsome-starter-bootstrap.svg)](https://greenkeeper.io/)

# Gridsome starter bootstrap

This is a starter project for Gridsome that comes with many features out of the box. It utilizes Bootstrap that is well known for powerful styling and layout. Ready to be deployed, automagically imports data to CMS and sets up your /admin page for easy access to edit your content.

It is designed to use Netlify, Forestry and Github which all have very fair free tier to their services, so you wont need to pay for monthly subscriptions and costly hosting fees.

### Demo

[https://gridsome-starter-bootstrap.loke.dev](https://gridsome-starter-bootstrap.loke.dev)

### Features

This starter project includes some of the latest powerful technologies.

*   **Gridsome -** Vue.js & GraphQL powered framework genrating static files.
*   **Bootstrap & Bootstrap Vue -** Powerful styling and layout with styled Vue components.
*   **Sass -** Professional grade CSS extension with many features.
*   **Forestry.io -** CMS that uses the Github repo for storage.
*   **Markdown -** Easy and widely used format for writing content.
*   **Netlify forms -** Netlify forms ready to be used after deployment.
*   **Google Analytics -** Just add your tracking ID in the config.
*   **Sitemap generator -** Automatically generates a sitemap.xml file.

### Getting started

The easiest way to get started quick is to use the Forestry button below, which will create a Github repository for you, clone this starter repo and import all data to the CMS. After that is complete, you can just go to [Netlify](https://www.netlify.com/) and connect your newly created project that will set it up for automatic deployment when you commit to the Github repo.

[![Import this project into Forestry](https://camo.githubusercontent.com/2455e97e4e989374a355fb0bea7ad364f2561c92/68747470733a2f2f6173736574732e666f7265737472792e696f2f696d706f72742d746f2d666f7265737472794b2e737667)](https://app.forestry.io/quick-start?repo=LokeCarlsson/gridsome-starter-bootstrap&provider=github&engine=vuepress) 

### Netlify config

Use the following build config for Netlify

Build command: `gridsome build`

Publish directory: `dist`

#### Manually install just the project (without CMS).

If you haven't already installed Gridsome CLI: `npm install --global @gridsome/cli`

1.  `gridsome create my-gridsome-site https://github.com/LokeCarlsson/gridsome-starter-bootstrap.git`
2.  `cd my-gridsome-site` to open folder
3.  `yarn dev` to start local dev server at `http://localhost:8080`
4.  Happy hacking 🎉🙌
