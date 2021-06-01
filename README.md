# Sudoers de Barcelona website

This is the source code for the website of the [Sudoers de Barcelona](https://barcelona.sudoers.io/), hosted at:

    https://barcelona.sudoers.io/
    
## How to publish the website

Changes to the `main` branch of this repository trigger a [GitHub workflow](https://github.com/sudoersbcn/sudoersbcn.github.io/blob/main/.github/workflows/gh-pages.yml), which generates the website content and commits it to the `gh-pages` branch of this repository.

## Powered by Hugo!

The website uses Hugo as static website generator, see [their website](https://gohugo.io/) for more information and for how to install and run it if needed.

The extended version of Hugo is required to build the site.

## How to test the website and changes on your own computer

The theme for the site is managed via a git submodule and it's tracking the `sudoersbcn` branch that implements some customizations over upstream version.
- Run `git submodule init` and `git submodule update`

To generate the static website, execute `hugo` to generate and serve the website on `localhost:1313`.

During development, it may be useful to run an incremental build. For this to work, execute `hugo server -D` to 
continuously (re)generate and serve the website on `localhost:1313`.

