# Personal Site

## Maintenance

- **Development**: This is a Quarto (v1.8.22 CLI) static site 
    - builds into `_sites/` folder as per the `_quarto.yml` 
    - Usually during development, we can use `quarto preview` to see changes live and iterate
- **Production**:
    - The end product is a GitHub pages site
    - The page is deployed by GitHub Actions using contents in the `docs/` folder
    - To build for production run `quarto render; cp -r _site/* docs/ -Force` in PowerShell (note different syntax for other OS), which renders into `_site/` then copies to `docs/`
    - Pushing to main will trigger GitHub actions to deploy the site

## Folders

### Posts

This is the blog posts folder. Each post is a separate `.qmd` file. The folder naming convention is `YYYY-MM-DD-title.qmd`.
