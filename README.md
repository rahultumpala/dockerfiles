This repo contains Dockerfiles with all the tools I need.  

Ubuntu - builds from ubuntu base with C++, Java, Go, Maelstrom and other basic dependencies.

To run: `docker run -it -v ./:/path_in_container ubuntu-dev-tooling`, this will open a bash session.

In Windows: `docker run -it -v /$(pwd):/path_in_container ubuntu-dev-tooling`, this will open a bash session.

To Mount a local dir `docker run -it -v /local_path:/container_path ubuntu-dev-tooling`
