# SBOL Standard Website

This repository contains the source for the SBOL Standard website, which is hosted at [sbolstandard.og](https://sbolstandard.org).

It uses the [Hugo static site generator](https://gohugo.io/) with [Wowchemy](https://wowchemy.com/).

Changes to the `master` branch trigger a GitHub action defined by [main.yml](https://github.com/SynBioDex/SbolStandardWebsite/blob/master/.github/workflows/main.yml).
This automatically rebuilds the site and pushes to the ` gh-pages` branch.
The [GitHub Pages configuration](https://github.com/SynBioDex/SbolStandardWebsite/settings/pages) specifies that the contents of the `gh-pages` branch are served on the `sbolstandard.org` domain.




## Contributing

Feel free to contribute by making a Pull Request. One of the SBOL Editors will review this, and merge if they approve.

You can also contribute by [creating an issue](https://github.com/SynBioDex/SbolStandardWebsite/issues/new/choose).

 

### Adding a Publication

To add a publication, create a new directory within [`content/publication`](https://github.com/SynBioDex/SbolStandardWebsite/tree/master/content/publication), and add two files:

* `cite.bib`, containing a citation [in BibTeX format](https://en.wikipedia.org/wiki/BibTeX)
* `index.md`, a markdown file containing details of the paper in a YAML metadata block

You can use one of the existing publications as a template.


### Adding a Tool

To add a software application or tool, create a new directory within [`content/applications`](https://github.com/SynBioDex/SbolStandardWebsite/tree/master/content/applications), and add an `index.md` file containing a description of the tool with details in a YAML metadata block.


### Adding a community member

To add a community member to the list on the [community page](https://sbolstandard.org/community/), edit the file [`contents/community/_index.md`](https://github.com/SynBioDex/SbolStandardWebsite/blob/master/content/community/_index.md)


### Adding a community event

To add a community event to the list on the [Community Meetings page](https://sbolstandard.org/community-meetings/), edit the file [`content/community-meetings/_index.md`](https://github.com/SynBioDex/SbolStandardWebsite/blob/master/content/community-meetings/_index.md)

Materials for community events (such as slides or example files) are stored in the separate [SynBioDex/Community-Media repository](https://github.com/SynBioDex/Community-Media)


## Building the site locally

### Without using docker

First install Hugo using the [official installation instructions](https://gohugo.io/getting-started/installing/).

Building the site requires Hugo to download some modules, so you will also need to [install Git](https://git-scm.com/downloads) and [install Go](https://go.dev/dl/).

You can then clone this repository:

    https://github.com/SynBioDex/SbolStandardWebsite.git

Change directory into the newly-created directory:

    cd SbolStandardWebsite

You can use the web-server built into Hugo to preview the effect of these changes by running:

    hugo server
    
and then opening [`http://localhost:1313/`](http://localhost:1313) in your preferred web browser.

#### Alternative to using the built-in server

Make the desired changes, and run:

    hugo

This will rebuild the site, saving the result in the `public/` subdirectory. You can preview this by running a webserver - see the [big list of HTTP static server one-liners](https://gist.github.com/willurd/5720255).

The contents of `public/` are ignored by the [`.gitignore`](https://github.com/SynBioDex/SbolStandardWebsite/blob/master/.gitignore) file: you should not force-add them to a commit as they will be automatically re-generated by the GitHub Action.


### Using Docker

If you have already [installed Docker](https://docs.docker.com/get-docker/), you may prefer to run Hugo inside a docker image rather than installing it on your host machine.

You can git clone the code from this repository:

    https://github.com/SynBioDex/SbolStandardWebsite.git

Change directory into the newly-created directory:

    cd SbolStandardWebsite

Make the desired changes, and re-build:

    docker run --rm -it -v $(pwd):/src --user $(id -u):$(id -g) klakegg/hugo:ext-alpine


## Checking for broken links

There is a Github Action which checks the deployed site for broken links.
This is not scheduled to run automatically on the first of the month, but additional runs can be triggered manually.

On the **Actions** tab, [select the "Check links on live website" action](https://github.com/SynBioDex/SbolStandardWebsite/actions/workflows/check-links.yml), then click "Run Workflow" to trigger a new run.

You cna view the results of an existing run from [the list of actions](https://github.com/SynBioDex/SbolStandardWebsite/actions/workflows/check-links.yml) by clicking on the "Check links on live website" title, and then on "check links".


## Problem solving

If you encounter problems, you may find the [Wowchemy website](https://wowchemy.com/) or [Discord channel](https://discord.com/invite/z8wNYzb) helpful.
