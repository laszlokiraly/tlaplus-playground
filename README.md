# tlaplus-playground

## Motivation
Playground Project for learning TLA+ from [The TLA+ Video Course](https://lamport.azurewebsites.net/video/videos.html)

## Prerequisites

- **Docker**
- **Visual Studio Code** with **Remote Containers** extension

## Setup

- clone repo
- open folder in **Visual Studio Code**
- `ctrl-shift-p` **Remote-Containers: Rebuild and Reopen in Container**
- test setup by
  - rightclicking **SimpleProgram.tla** and selecting **Check model with TLC**: Status should be green/success
  - selecting **SimpleProgram.tla** and `ctrl-shift-p` **TLA+: Export module to PDF**

## References

- [Dockerfile](https://github.com/hackenfreude/docker-tlatoolbox-1.5.2)
- eventually https://github.com/tlaplus-workshops/ewd998