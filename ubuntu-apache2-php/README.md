# Docker Images

Repository to contain the build process for public docker images. Each directory has the same name as an image.

This project was based on [Docker-Images project from TallweWebSolutions] (https://github.com/TallerWebSolutions/docker-images)

## Commands# Docker Images

Repository to contain the build process for public docker images built by the Taller team. Each directory has the same name as an image.

This project was based on [Docker-Images project from TallweWebSolutions](https://github.com/TallerWebSolutions/docker-images)

## Commands

These are shortcut commands available with `make` inside each image directory:

- `run`: Run a container for testing purpose.
- `pull`: Pulls the image.
- `build`: Builds the image.
- `push`: (deprecated) Builds and pushes the image.

These are common arguments available:

Argument | Default             | Description
---------|--------------|-------------------
TAG      | stable              | Image tag to build
USER     | taller              | The Docker user name
REPO     | $(notdir $(CURDIR)) | The repository name


## Customization

Here are some tips to customizing the images for each project's needs.

### Timezone

To set timezone configuration, use the environment variable TZ. [Read more](https://github.com/docker/docker/issues/12084#issuecomment-160177087).

## LICENSE
MIT