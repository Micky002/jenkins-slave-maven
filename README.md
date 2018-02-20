[![Build Status](https://img.shields.io/docker/build/wemicky/jenkins-slave-maven.svg)](https://hub.docker.com/r/wemicky/jenkins-slave-maven/)

Jenkins jnlp slave with maven included

## How to use

Start the container

    docker run wemicky/jenkins-slave-maven:latest -url http://jenkins-server:port <secret> <agent name>

For the detached mode use the -d option.

    docker run -d wemicky/jenkins-slave-maven:latest -url http://jenkins-server:port <secret> <agent name>

Set the name of the container with the --name <name> argument.

    docker run --name <container name> wemicky/jenkins-slave-maven:latest -url http://jenkins-server:port <secret> <agent name>

## Options

To use more custom options see the base image [jenkinsci/jnlp-slave](https://github.com/jenkinsci/docker-jnlp-slave).
