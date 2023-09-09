# docker-desktop-netbeans-ide

## Description
This is a POC project to demonstrate netbeans an integrated development environment for java programming.

This is a barebones installation no pluggins where added. That said, by default gradle and maven are installed by default

In order to be able to get files out of the container one must add a *volume* to the docker run command.

ie.
without a volume
`docker run --rm` ...
with a volume
`docker run --rm -v $(pwd):/app` ...

Supports X11 display forwarding from docker container.

## Tech stack
- netbeans
- java
    - ant
    - gradle
    - maven

## Docker stack
- ubuntu:18.04

## To run
`sudo ./install.sh -u`

## To stop (optional)
`sudo ./install.sh -d`

## To see help
`sudo ./install.sh -h`
