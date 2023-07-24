# Starting new instance.

Fastgeoapi is a bundle of multiple applications working together, which means it can be plugged into existing architecture or created entirely from scratch as well.

## Instance from scratch

We'll be assuming that none of the required libraries and packages are available in the system as of now. 

### Cloning and setting up code

Clone this [fastapi](https://github.com/geobeyond/fastgeoapi) repo on your local machine. This repo consists of package file maintained by [Poetry](https://python-poetry.org/). Once the cloning is successful open folder in terminal and type 

```console
poetry shell
```

which will create python environment, inside which execute 

```console
poetry install
```

which will install all required packages.

### Setting up docker

Few requirements (OIDC server and keycloak) are managed by docker, the script for the same is available at `scripts/iam/docker-compose.yml`, open this folder path on another terminal and execute

```console
docker-compose up -d
```