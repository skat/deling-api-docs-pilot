# DELING API Documentation

This is a site for providing documentation for the pilot project DELING API. It is hosted at https://skat.github.io/deling-api-docs.

The documentation is written with [API Blueprint](https://apiblueprint.org/) for the DELING project.

The framework is provided by [aglio](https://github.com/danielgtaylor/aglio), and converts the [`deling-api.md`](deling-api.md) to html.

## Updating content

Update the documentation file [`deling-api.md`](deling-api.md), and open a pull request to suggest changes.

## Running documentation locally

To run the documentation locally you should have this repository checked out.

### Installing dependencies
```
npm install -g aglio
```

### Preview changes
```
aglio -i deling.api.md -s
```
### Publishing changes
The master branch is published as a GitHub page. It is published when a new change to `index.html` is pushed to master. To update `index.html`, run:
```
 aglio --theme-variables flatly -i deling-api.md --theme-template triple  -o index.htm
```