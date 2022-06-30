# Bridge Foundry Operations Guide

Welcome to the Operations Guide for Bridge Foundry, Inc.,
a US non-profit organization with a 501c3 designation.

Our open source and online resources are freely available to anyone for use
in furthering our mission. This support of independent communities all over the
world is governed by open source license agreements and terms of service.

For details about who runs our operations and writes this guide, see [CONTRIBUTING](CONTRIBUTING.md)

## About mkdocs + operations.bridgefoundry.org

operations.bridgefoundry.org uses `mkdocs` to turn this git repository
into well-formatted HTML. You can run `mkdocs` on your own computer to
preview the site.

We use GitHub Actions to generate the site when the
`main` branch updates; Build logs can be found
[here](https://github.com/bridgefoundry/operations/actions/workflows/build.yml).

We use GitHub Pages to serve the website to the world.

## Running Locally
To generate the nicely-formatted site on your own computer, open up a
terminal app and navigate to the folder with the operations
guide.

1. Install Python and pip: [get-pip.py](https://packaging.python.org/tutorials/installing-packages/)

2. Install virtualenv and `mkdocs`
```
pip install virtualenv
virtualenv tmp/docs-virtualenv
tmp/docs-virtualenv/bin/pip install mkdocs
```

3. run the website locally:
```
tmp/docs-virtualenv/bin/mkdocs serve
```

Now **http://127.0.0.1:8000** should contain a live preview of the
website.

## Formatting with mkdocs
Here are the special things that mkdocs needs to display the markdown appropriately:

- New line between a paragraph and bullet points in order for bullet points to display
- Four spaces before a sub-bullet (rather than 2 spaces)
   - Like this!
