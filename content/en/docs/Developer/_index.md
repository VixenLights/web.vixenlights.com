---
title: Developer
weight: 100
type: docs
aliases: [/docs/contribution-guidelines]
menu:
  main:
    weight: 100
description: How to contribute to Vixen
---

Vixen is an open source project and we love getting patches and contributions to make Vixen and its docs even better.

## Contributing to Vixen

The Vixen code itself lives in <https://github.com/vixenlights/vixen>.

### Contributor License Agreement

Contributions to this project become part of the project and are subject to the open source licensing.

### Code reviews

All submissions, including submissions by project members, require review. We
use GitHub pull requests for this purpose. Consult
[GitHub Help](https://help.github.com/articles/about-pull-requests/) for more
information on using pull requests.

### Community guidelines

This project follows
[Google's Open Source Community Guidelines](https://opensource.google.com/conduct/).

### Creating issues

Alternatively, if there's something you'd like to see in Vixen (or if you've found something that isn't working the way you'd expect), but you're not sure how to fix it yourself, please create an [issue](https://bugs.vixenlights.com).

## Contributing to these docs

This user guide is a Docsy site that uses the Hugo static site generator. We welcome updates to the docs!

### Updating a single page

If you've just spotted something you'd like to change while using the docs, Docsy has a shortcut for you:

1. Click **Edit this page** in the top right hand corner of the page.
1. If you don't already have an up to date fork of the project repo, you are prompted to get one - click **Fork this repository and propose changes** or **Update your Fork** to get an up to date version of the project to edit. The appropriate page in your fork is displayed in edit mode.

### Previewing your changes locally

If you want to run your own local Hugo server to preview your changes as you work:

1. Follow the instructions in [Getting started](/docs/getting-started) to install Hugo and any other tools you need.
1. Fork the [Vixen Website](https://github.com/vixenlights/web.vixenlights.com) repo into your own project, then create a local copy using `git clone`:

    ```sh
    git clone git@github.com:VixenLights/web.vixenlights.com.git
    ```

1. Change to the `web.vixenlights.com` directory and run the following Hugo command to build the site and start the Hugo server.

    ```sh
    cd web.vixenlights.com
    hugo server
    ```

    By default your site will be available at http://localhost:1313/. Now that you're serving your site locally, Hugo will watch for changes to the content and automatically refresh your site.

2. Continue with the usual GitHub workflow to edit files, commit them, push the
  changes up to your fork, and create a pull request.

### Creating an issue

If there's something you'd like to see in the docs, but you're not sure how to fix it yourself, please create an issue in [this repository](https://github.com/vixenlights/we/vixenlights.com). You can also create an issue about a specific page by clicking the **Create Documentation Issue** link in the top right hand corner of the page.
