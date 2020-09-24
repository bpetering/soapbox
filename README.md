# soapbox
A tool for static-site publishing in Python.

## Overview
This is an opinionated, minimalist tool used to publish [benpetering.com](benpetering.com). It's a single Python file, and doesn't even have any dependencies except [Jinja](https://jinja.palletsprojects.com/), to provide a template engine.

It supports:
* generating both HTML pages and posts from templates
* `build` action, to rebuild the entire site
* `view` action, to view the site in a local web server

It doesn't support:
* publishing logic (SSH/rsync/FTP)
* rebuilding while the web server is running (TODO)

## Usage

`python soapbox.py build`

... then, to test your build:

`python soapbox.py view`

Once you're happy, copy the `~/soapbox/build` directory contents to your domain's docroot.



