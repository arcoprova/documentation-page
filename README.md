# Jupiter FOSS fpm template

[![Deploy Site](https://github.com/FifthTry/jupiter-foss-template/actions/workflows/deploy.yml/badge.svg)](https://github.com/FifthTry/jupiter-foss-template/actions/workflows/deploy.yml)

This template allows you to get started with building a website for your FOSS  using [`fpm`](https://fpm.dev).


## Getting started with this template

This template provides you everything you need to get started with an FPM package.

### Deploying the package

The package can be deployed in multiple ways.

#### How does the deployment work

FPM builds a static site for you to serve from any static site hosting service. 
You can use the standard [github pages](https://pages.github.com/) service or any 
other third party service to serve your application.

The `deploy` action is triggered whenever any change is made to the `ftd` document 
in the repository. The action generates 2 branches which can be deployed right away.

- `gh-pages` branch: This branch is generated primarialy for deploying on github in a 
  namespaced URL <username/org>.github.io/<repo-name>/...
  The static site built in this branch will have the `<repo-name>` as the prefix for 
  all the links while building.
- `build` branch: Use this branch to do a TLD hosting.

##### Github Pages

For enabling the github pages, please head over to `Pages` section in your repository 
settings and choose the `gh-pages` branch to host the website.

If you want to use a custom domain for your repository, it's suggested that you use the 
`build` branch to deploy the changes.

##### Vercel

Head over to vercel and attach the appropriate repository's `build` branch to get started.