# Tetrifact Build

Build container for the Tetrifact project. Use for unit testing and building in container-based CI systems.

Hosted at https://hub.docker.com/r/shukriadams/tetrifact-build

Tetrifact : https://github.com/shukriadams/tetrifact

## Build

sh ./build.sh

## Test

After building, confirm dotnet core is working with

    docker-compose up -d
    docker exec -it tetrifact-build bash
    dotnet
