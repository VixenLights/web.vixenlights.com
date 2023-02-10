---
title: Contribute to Documentation
author: Vixem Team
weight: 20
description: How to contribute to the Vixen documentation.
---

### Overview

Vixen is an open source project and we love getting patches and contributions to make Vixen and its docs even better.

This user guide is a Docsy themed site that uses the Hugo static site generator. The code for the website is hosted on [Github][5].

We welcome updates to the docs!

### Updating a single page

If you've just spotted something you'd like to change while using the docs, Docsy has a shortcut for you:

1. Click **Edit this page** in the top right hand corner of the page.
2. If you don't already have an up to date fork of the project repo, you are prompted to get one - click **Fork this repository and propose changes** or **Update your Fork** to get an up to date version of the project to edit. The appropriate page in your fork is displayed in edit mode.
3. Submit a pull request to the develop branch in the repository and it will be reviewed for inclusion.

### Previewing your changes locally

If you want to run your own local Hugo server to preview your changes as you work:

1. Follow the instructions in [Docsy Getting Started][6] to install Hugo and any other tools you need.
2. Fork the [Vixen Website][5] repo into your own project, then create a local copy using `git clone`:

    ```sh
    git clone git@github.com:VixenLights/web.vixenlights.com.git
    ```

3. Change to the `web.vixenlights.com` directory and run the following Hugo command to build the site and start the Hugo server.

    ```sh
    cd web.vixenlights.com
    npm install
    hugo server
    ```

    By default your site will be available at http://localhost:1313/. Now that you're serving your site locally, Hugo will watch for changes to the content and automatically refresh your site.

4. Continue with the usual GitHub workflow to edit files, commit them, push the
  changes up to your fork, and create a pull request.

### Creating an issue

If there's something you'd like to see in the docs, but you're not sure how to fix it yourself, please create an [Issue][7] on Github for this repository. You can also create an issue about a specific page by clicking the **Create Documentation Issue** link in the top right hand corner of the page.

[5]: https://github.com/vixenlights/web.vixenlights.com
[6]: https://www.docsy.dev/docs/get-started/
[7]: https://github.com/VixenLights/web.vixenlights.com/issues/new
