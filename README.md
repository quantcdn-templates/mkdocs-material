# MkDocs (Material theme) QuantCDN starter template

![Template screenshot](quant/screenshot.png?raw=true)

This starterkit provides a simple MkDocs codebase using the popular [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme.

Click the "Deploy to Quant" button to create a new repo, QuantCDN project, and deployment pipelines.

[![Deploy to Quant](https://www.quantcdn.io/img/quant-deploy-btn-sml.svg)](https://dashboard.quantcdn.io/deploy/step-one?template=mkdocs-material)

### Local Development

This project ships with a Dockerfile and docker-compose for simple local development.

```
$ docker-compose up
```

This command starts a local development server. You can view your docs site at http://localhost:8000/. Changes made to documentation or theme will preview live on your browser.

### Build

```
$ docker-compose exec mkdocs mkdocs build
```

This command generates static content into the `site` directory and can be served using any static hosting service.

### Deployment

#### Locally

If Quant CLI is configured (e.g via `quant init`) then you can simply run the following to deploy the latest build to Quant.

```
quant deploy
```

#### via CI

This template automatically preconfigures your CI pipeline to deploy to Quant. This means you simply need to edit content and commit changes to trigger the build & deploy process.