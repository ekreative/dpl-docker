# Dpl docker image

Image used for running [dpl](https://github.com/travis-ci/dpl)

Also includes `aws-sdk-v1` gem because we are using the OpsWorks provider and including it makes things faster

## Build command

    docker build -t ekreative/dpl .

## Build an app

    docker run -ti --rm --volume=$(pwd):/opt/workspace ekreative/dpl dpl --provider=...
