# VuePress Blog Boilerplate



This is an ever-changing and opinionated architecture that uses [VuePress](https://vuepress.vuejs.org) to power your blogging platform.

## Purpose

To provide a blueprint of how blogging is possible with [VuePress](https://vuepress.vuejs.org/) and empower you with enough boilerplate so you feel comfortable customizing it to your liking.

## Features

- Write posts in Markdown
- Basic pagination sorted by most recent posts
- Ability to search for posts via headings within the post
- Archived posts page
- Basic scheduling for future publishing
- Basic tagging for posts
- Automatic RSS feed generation
- Easily integrate Google Analytics

## Getting Started

### Prerequisites

- [NodeJS >= 8](https://nodejs.org/)
- [yarn](https://yarnpkg.com/lang/en/docs/install/) (Recommended)
- Basic knowledge of navigating the terminal

### Installation

clone repo

```bash

# Change directory into project
cd <dir>

# Install dependencies
yarn

# Run local server
yarn dev
```

You should now be able to visit [http://localhost:8080](http://localhost:8080)!

## Documentation

To check out the tutorial and docs, check out [the guide](https://vuepress-blog-boilerplate.bencodezen.io/).

## Examples

- [Blog](https://wjv.io/blog)


## Git Push & Deployment with Travis CI

The Local repo contains the development platform for Vuepress where all changes to posts/styles/etc are to be made. To check that the Travis CI deployment will be successful, first, in your dev branch, be sure to run 
```
npm run docs:build
```
Correct any errors here before pushing.

When satisfied with changes you must `git push --force` if on master or `git push origin dev` if on dev branch. to trigger Travis CI to rebuild the branch and deploy it to Github pages. Do not `git pull` from origin as that will pull down only the built `/dist` folder contents that Travis CI deployed last.
