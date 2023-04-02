# Welcome to MkDocs

This starterkit provides a simple MkDocs codebase using the popular [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme.

Your documentation will automatically be built and deployed to [QuantCDN](https://www.quantcdn.io) via GitHub actions.

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `docker-compose up` - Run the project locally
* `docker-compose exec mkdocs mkdocs build` - Build the static docs output (built into the `site` folder)

## QuantCDN integration

Any documentation change made in the `master` branch will automatically build and deploy to your QuantCDN project via a GitHub actions pipeline. Check the `.github/workflows/ci.yml` file for more detail.


## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.
