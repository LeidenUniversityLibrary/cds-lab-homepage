# CDS Lab Homepage

This repository contains the source files for the [CDS Lab (homepage)](https://lab.library.universiteitleiden.nl/).
The website is built with [MkDocs](https://www.mkdocs.org) plus plugins and a theme.

## Build locally

To install MkDocs and the plugins and theme, so that you can build the website, you need Python 3.6+ installed and run the following commands:

```
pip3 install -r requirements.txt
mkdocs build
```

Note: you may need to call `pip` instead of `pip3` depending on your system.

## Deploy to the Web

When the site is built, the HTML output is written to the `./site/` directory by default.
We currently deploy the website by `rsync`ing to the right directory on the web server.

Alternatively, we can use `mkdocs gh-deploy`. This command builds the site and stores the output
on the `rendered` branch and pushes the branch to the remote (i.e. GitHub).
Then, on the server, we can `git pull` the `rendered` branch and copy the files to the
web directory.
