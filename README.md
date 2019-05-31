# The Pulter Project Central

## Welcome
This repository contains everything (well, almost, [see below](#where-are-all-the-images)) that the project needs to live and grow.

## For the Editors
These are the folders of the utmost interest for the contributing parties, as well as the editors:
* `/pulter-poems` — TEI XML encoded poems, the gold;
* `/pulter-site/pages` — static pages of the site;
* `/pulter-site/curations` — poem curations (HTML pages);
* `/pulter-site/explorations` — explorations (HTML pages).

## For the Developers
### How to Start
1. Make sure your machine has [Node.js](https://nodejs.org/en/) as well as [Java 6 runtime](https://support.apple.com/kb/dl1572?locale=en_US) installed.
2. Install gulp-cli tool globally: `npm install gulp-cli -g`.
3. Run `npm install`.

You should have the following terminal commands available:
* `gulp` — boots up the development web server with automatic JS/CSS compilation and browser reloading; this it the default mode for active development;
* `gulp xslt:poems` — builds an array of HTML pages representing the whole corpus of the poems and their editions; this will generate the structure that will live under `/poems`;
* `gulp xslt:manifest` — builds JSON manifest (`/pulter-manifest.json`) of the poems
* `gulp xslt:index` — builds the main index page
* `gulp xslt:lunr` — builds the search functionality
* `gulp xslt` — runs all the commands from `xslt` namespace; re-compiles the whole site;
* `gulp deploy` — builds a production version of the site and puts it in `/dist`.
