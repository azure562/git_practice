---
title: "Automate Hugo Deployment to GitHub Page"
date: 2021-09-25T19:35:32+02:00
slug: ""
description: ""
keywords: []
tags: ["Hugo", "Workflow", "Automation"]
math: false
toc: false
---

Setting up a blog under your own control might sound tricky, unless you know the secret ... Mine is [Hugo](https://gohugo.io/) + [GitHub Pages](https://pages.github.com/).

There are lots of helpful articles available online, a proof that many people have tried it out.

Below is a summary of my approach:

1. Set up a repository for the source content.

2. Set up another repository for the GitHub page, which will host your generated website.

    For these first two steps, you can aslo follow [Build a Personal Website With Github Pages and Hugo](https://levelup.gitconnected.com/build-a-personal-website-with-github-pages-and-hugo-6c68592204c7).

3. Automate the deployment using GitHub Actions.

    Create a yaml file in your GitHub folder `workflows` (my workflow is [here](https://github.com/azure562/retold-source/blob/master/.github/workflows/gh-pages.yml)).

    The most important job is, surprise, surprise, named `Deployment`.

    ```
    - name: Deploy
      uses: peaceiris/actions-gh-pages@v3.8.0
      with:
        personal_token: ${{ secrets.PERSONAL_TOKEN }}
        external_repository: azure562/azure562.github.io # Replace with your own GitHub Page repo
        publish_branch: master
        publish_dir: ./public
    ```

Note the following:

* The generated website is hosted in a different repository, which means you need to [Deploy to external repository](https://github.com/peaceiris/actions-gh-pages#%EF%B8%8F-deploy-to-external-repository-external_repository)

* To access external repository, you need to [Set Personal Access Token personal_token](https://github.com/peaceiris/actions-gh-pages#%EF%B8%8F-set-personal-access-token-personal_token). See also [Creating a personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token).

* It makes sense to publish to the main branch, which is `master` in my repo.

If you are reading this as a blog post, then it means *it works*! 🎉