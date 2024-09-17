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
RUN apt-get install -y elixir

ENTRYPOINT "/bin/bash"
