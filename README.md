# Example Voting App

A simple distributed application running across multiple Docker containers.

## Architecture
* A front-end web app in [Python](/vote) which lets you vote between two options
* A [Redis](https://hub.docker.com/_/redis/) which collects new votes
* A [.NET](/worker/) worker which consumes votes and stores them in…
* A [Postgres](https://hub.docker.com/_/postgres/) database backed by a Docker volume
* A [Node.js](/result) web app which shows the results of the voting in real time

## Polyglot/Heterogenous Microservices

This project is to demo an application with heterogenous Microservices built using different technologies and yet can be embeded into a single repository.   
The path based triggering of the pipeline lets you deploy/update individual microservices in the cluster without impacting each other.   
For details please check the pipeline steps: [.github/workflows](.github/workflows)


