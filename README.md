# docker-demo

# Docker Usage Guide

This README provides basic instructions on how to install, configure, and use Docker.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Docker Basics](#docker-basics)
  - [Common Commands](#common-commands)
  - [Working with Images](#working-with-images)
  - [Running Containers](#running-containers)
- [Dockerfile](#dockerfile)
- [Volumes](#volumes)
- [Networking](#networking)
- [Docker Compose](#docker-compose)
- [Resources](#resources)

## Prerequisites

Before using Docker, ensure the following are in place:

1. A machine with Docker installed (Linux, macOS, or Windows).
2. Basic understanding of command line usage.

## Installation

### On Linux:

```bash
# Update the package database
sudo apt-get update

# Install necessary packages
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common

# Add Docker’s official GPG key
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

# Add the Docker APT repository
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

# Update the package database with Docker packages from the newly added repo
sudo apt-get update

# Install Docker
sudo apt-get install docker-ce

# Verify Docker is installed and running
sudo systemctl status docker
