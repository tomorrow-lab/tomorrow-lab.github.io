# Blog

# Tools

- quarto

# useful command

```
quarto preview
```


# Publishing 
There are a wide variety of ways to publish documents, presentations, and websites created using Quarto. Since content rendered with Quarto uses standard formats (HTML, PDFs, MS Word, etc.) it can be published anywhere. Additionally, there is a quarto publish command available for easy publishing to various popular services (GitHub, Netlify, Posit Connect, etc.) as well as various tools to make it easy to publish from a Continuous Integration (CI) system.

GitHub Pages is a website hosting service that enables you to publish content based on source code managed within a GitHub repository.

There are three ways to publish Quarto websites and documents to GitHub Pages:

Render sites on your local machine to the docs directory, check the rendered site into GitHub, and then configure your GitHub repo to publish from the docs directory.

Use the quarto publish command to publish content rendered on your local machine.

Use a GitHub Action to automatically render your files (a single Quarto document or a Quarto project) and publish the resulting content whenever you push a source code change to your repository.

We’ll cover each of these methods below, but first an important pre-requisite: you need to have a Git repository on your local machine that is synced to GitHub. The URL of the published website will be derived from the combination of your username and the repository name (e.g. https://username.github.io/reponame/).

You can optionally configure a custom domain for a GitHub Pages site, but before exploring that ground you should get your site up and running with the default domain.

## Publishing

Once you have configured the source branch and updated your .gitignore, navigate to the directory where your project / git repository is located, make sure you are not on the gh-pages branch, and execute the quarto publish command for GitHub Pages:

```
quarto publish gh-pages
```

The publish command will confirm that you want to publish, render your content, copy the output to a special gh-pages branch, push that branch to GitHub, and then open a browser to view your site once it is deployed.

## User Site
In addition to creating sites tied to various repositories, you can also create a user site that is served from your root user domain (e.g. https://username.github.io). This is an ideal place to publish a blog or personal home page. To create a user site:

Create a Git repo with the name username.github.io (where “username” is your GitHub username) and sync it to your local machine.

Set the Source branch for your user site to gh-pages as described in Source Branch.

# 참고용 사이트

- https://publickrbook.com/
- https://www.lostineconomics.com/