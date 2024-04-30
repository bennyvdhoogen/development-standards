# Coding standards for the developers of the city of Amsterdam

Team responsible : Engineering Enablement team

## Aims of this repo
This repository strives to offer a comprehensive overview of the standards presently utilized within the developer community at the municipality of the city of Amsterdam. Additionally, it encompasses a summary of both rejected and under-review standards. You can access the overview by following this link. //TODO write a link to the Amsterdam tech-radar page

## How to use this repo?
Within the "General" folder, you will find descriptions of standards that apply regardless of whether you identify as a back- or front-end developer. In the "Backend" and "Frontend" folders, you can locate standards specifically tailored for each respective group of developers.
If a standard is labeled as a recommendation, it indicates that it is not widely embraced by our developer community.

## How to contribute to this repo?
If you would like to include additional standards, please refer to the manual for instructions on implementing new standards. (TODO: Create a link to the implementation page of standards.) If you have any other matters to bring to our attention, you can contact us via Teams (DV - Engineering Enablement) or Slack (#engineering-enablement).









# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

### Installation

```
$ yarn
```

### Local Development

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:

```
$ USE_SSH=true yarn deploy
```

Not using SSH:

```
$ GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
