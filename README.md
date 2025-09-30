# UCL MIRSG Docs

Public facing documentation for MIRSG and our services. Built with
[Material for MkDocs](https://github.com/squidfunk/mkdocs-material) and deployed
to <https://ucl-mirsg.github.io/docs/>

## Build & Deployment

### Production

This repository runs
[deploy_site.yml](https://github.com/UCL-MIRSG/docs/blob/main/.github/workflows/deploy_site.yml)
GitHub workflow on the `main` branch to to build the contents of the `docs`
folder and push it to
[`gh-pages`](https://github.com/UCL-MIRSG/docs/tree/gh-pages) branch.

Deployment is then through GitHub Pages using the
[Publishing from a branch](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#publishing-from-a-branch)
mechanism. Manual pushes to the `gh-pages` branch should never be needed.

### Local Preview

To preview locally as you develop you will need to do the following:

1. Create a Python virtual environment and install the dependencies listed in
   [`pyproject.toml`](./pyproject.toml). (e.g. by using `uv`)
2. Run `mkdocs serve` from the project root to
   [preview as you write](https://squidfunk.github.io/mkdocs-material/creating-your-site/#previewing-as-you-write).

## Contributing

We welcome contributions from UCL and external users, as well as wider team
members to these docs. Please see the [Contributing Guide](./CONTRIBUTING.md)
for details.
