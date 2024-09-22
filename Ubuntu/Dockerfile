# our local base image
FROM ubuntu:latest

LABEL description="Container with personal dev tooling"

RUN apt-get update

# install basic dependencies
RUN apt-get install -y g++ rsync zip openssh-server make git vim

# for blog
RUN apt-get install lowdown

# for dist-sys challenges
RUN apt-get install -y gnuplot graphviz maelstrom golang-go openjdk-11-jdk

# for hackattic challenges I'm solving using elixir
ARG hackattic_token
ENV hackattic_access_token $hackattic_token
RUN apt-get install -y elixir
RUN mix local.hex --force

# c++ deps
RUN apt-get install -y openssl libssl-dev --fix-missing

ENTRYPOINT "/bin/bash"